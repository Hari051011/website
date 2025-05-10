# Ex.07 Restaurant Website
# Date:09/05/2025
# AIM:
To develop a static Restaurant website to display the food items and services provided by them.

# DESIGN STEPS:
## Step 1:
Requirement collection.

## Step 2:
Creating the layout using HTML and CSS.

## Step 3:
Updating the sample content.

## Step 4:
Choose the appropriate style and color scheme.

## Step 5:
Validate the layout in various browsers.

## Step 6:
Validate the HTML code.

## Step 7:
Publish the website in the given URL.

# PROGRAM:
index.html
```

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Home - The B & I's</title>
  <link rel="stylesheet" href="home.css">
</head>
<body>
  <header>
    <h1>Welcome to The B & I's</h1>
  </header>
  <nav>
    <a href="index.html">Home</a>
    <a href="menu.html">Menu</a>
    <a href="admin.html">Administration</a>
    <a href="contact.html">Contact Us</a>
  </nav>
  <div class="banner"></div>
  <div class="container">
    <h2>About Us</h2>
    <p>We serve the most delicious food in town using only the freshest ingredients.</p>
  </div>
  <footer>
    <p>Website designed by HARI KRISHNAN</p>
  </footer>
</body>
</html>

```
home.css
```
body {
    margin: 0;
    font-family: Arial, sans-serif;
    background-image: url('bg.jpg');
    background-size: cover;
    background-repeat: no-repeat;
    background-attachment: fixed;
    background-position: center;
    color: #fff;
    min-height: 100vh;
    display: flex;
    flex-direction: column;
  }
  
  .container {
    width: 90%;
    max-width: 800px;
    margin: 30px auto;
    background-color: rgba(0, 0, 0, 0.6); /* semi-transparent bg */
    padding: 20px;
    border-radius: 10px;
  }
  
  header, nav, footer {
    text-align: center;
    padding: 20px;
  }
  
  nav {
    background-color: rgba(255, 255, 255, 0.2);
  }
  
  nav a {
    color: #fff;
    text-decoration: none;
    margin: 0 15px;
    font-weight: bold;
  }
  
  footer {
    background-color: rgba(0, 0, 0, 0.6);
  }
  ```
  menu.html
  ```
  <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Menu</title>
  <link rel="stylesheet" href="menu.css">
</head>
<body>
  <header>
    <h1>Our Menu</h1>
  </header>
  <nav>
    <a href="index.html">Home</a>
    <a href="menu.html">Menu</a>
    <a href="admin.html">Administration</a>
    <a href="contact.html">Contact Us</a>
  </nav>
  <div class="container">
    <div class="menu-grid">
      <div class="item">
        <img src="bc.jpg" alt="Butter Chicken">
        <h3>Butter Chicken</h3>
        <p>Rs.320</p>
      </div>
      <div class="item">
        <img src="pt.jpg" alt="Paneer Tikka">
        <h3>Paneer Tikka</h3>
        <p>Rs.280</p>
      </div>
      <div class="item">
        <img src="cp.jpg" alt="Cheese Burst Pizza">
        <h3>Cheese Burst Pizza</h3>
        <p>Rs.449</p>
      </div>
      <div class="item">
        <img src="ml.jpg" alt="Masala Dosa">
        <h3>Masala Dosa</h3>
        <p>Rs.150</p>
      </div>
      <div class="item">
        <img src="sr.jpg" alt="Spring Rolls">
        <h3>Spring Rolls</h3>
        <p>Rs.200</p>
      </div>
      <div class="item">
        <img src="biri.jpg" alt="Chicken Biryani">
        <h3>Chicken Biryani</h3>
        <p>Rs.350</p>
      </div>
      <div class="item">
        <img src="vt.jpg" alt="Veg Thali">
        <h3>Veg Thali</h3>
        <p>Rs.270</p>
      </div>
      <div class="item">
        <img src="gb.jpg" alt="Garlic Bread">
        <h3>Garlic Bread</h3>
        <p>Rs.160</p>
      </div>
      <div class="item">
        <img src="mj.jpg" alt="Mint Mojito">
        <h3>Mint Mojito</h3>
        <p>Rs.99</p>
      </div>
      <div class="item">
        <img src="gj.webp" alt="Gulab Jamun">
        <h3>Gulab Jamun</h3>
        <p>Rs.80</p>
      </div>
      <div class="item">
        <img src="ml.jpg" alt="Mango Lassi">
        <h3>Mango Lassi</h3>
        <p>Rs.70</p>
      </div>
      <div class="item">
        <img src="br.jpg" alt="Chocolate Brownie">
        <h3>Chocolate Brownie</h3>
        <p>Rs.120</p>
      </div>
    </div>
  </div>
  <footer>
    <p>Website designed by HARI KRISHNAN</p>
  </footer>
</body>
</html>
```
menu.css
```
/* Global Styles */
body {
  font-family: 'Segoe UI', sans-serif;
  background-color: #fdf6ec;
  margin: 0;
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}

header {
  background-color: #8B0000;
  color: white;
  padding: 20px;
  text-align: center;
}

nav {
  background-color: #eee;
  text-align: center;
  padding: 12px;
}

nav a {
  margin: 0 20px;
  text-decoration: none;
  color: #8B0000;
  font-weight: 600;
  transition: color 0.3s ease;
}

nav a:hover {
  color: #FF6347;
}

.container {
  padding: 30px 20px;
  flex: 1;
}

/* Menu Grid */
.menu-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 24px;
}

.item {
  background-color: white;
  padding: 15px;
  text-align: center;
  border: 0.5px solid rgba(0, 0, 0, 0.1); /* Thin border */
  border-radius: 12px;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.05);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.item:hover {
  transform: translateY(-6px);
  box-shadow: 0 6px 15px rgba(0, 0, 0, 0.1);
}

.item img {
  width: 100%;
  height: 180px;
  object-fit: cover;
  border-radius: 8px;
}

.item h3 {
  margin: 12px 0 6px;
  font-size: 1.2rem;
  color: #333;
}

.item p {
  margin: 0;
  font-weight: bold;
  color: #555;
}

/* Responsive Design */
@media (max-width: 768px) {
  .menu-grid {
    grid-template-columns: repeat(2, 1fr);
  }
}

@media (max-width: 480px) {
  .menu-grid {
    grid-template-columns: 1fr;
  }
}

/* Footer */
footer {
  background-color: #8B0000;
  color: white;
  text-align: center;
  padding: 12px;
  font-size: 0.9rem;
}
```
admin.html
```

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Administration</title>
<link rel="stylesheet" href="admin.css">
</head>
<body>
<header>
  <h1>Our Team</h1>
</header>
<nav>
  <a href="index.html">Home</a>
  <a href="menu.html">Menu</a>
  <a href="admin.html">Administration</a>
  <a href="contact.html">Contact Us</a>
</nav>
<div class="container">
  <div class="team">
    <!-- Repeat for 6 members -->
    <div class="member">
      <img src="mr.jpg" alt="Chef">
      <h3>Madhampatty rangaraj</h3>
      <p>Head Chef</p>
    </div>
    <div class="member">
      <img src="jane.jpg" alt="Chef">
      <h3>Jane Smith</h3>
      <p>Chef</p>
    </div>
    <div class="member">
      <img src="manager.jpg" alt="Manager">
      <h3>Jenifer</h3>
      <p>Manager</p>
    </div>
    <div class="member">
      <img src="john.jpg" alt="Chef">
      <h3>John</h3>
      <p>Chef</p>
    </div>
    <!-- 4 more -->
  </div>
</div>
<footer>
  <p>Website designed by HARI KRISHNAN</p>
</footer>
</body>
</html>

```
admin.css
```
body {
  font-family: sans-serif;
  background-color: #f9f9f9;
  margin: 0;
}

header, footer {
  background-color: #8B0000;
  color: white;
  text-align: center;
  padding: 20px 10px;
}

nav {
  background-color: #ddd;
  text-align: center;
  padding: 10px;
}

nav a {
  margin: 0 15px;
  text-decoration: none;
  color: #8B0000;
}

.container {
  padding: 20px;
}

.team {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 20px;
}

.member {
  background: white;
  padding: 10px;
  text-align: center;
}

.member img {
  width: 100%;
  height: 200px;
  object-fit: cover;
}
```
contact.html
```
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Contact Us</title>
<link rel="stylesheet" href="contact.css">
</head>
<body>
<header>
  <h1>Contact Us</h1>
</header>
<nav>
  <a href="index.html">Home</a>
  <a href="menu.html">Menu</a>
  <a href="admin.html">Administration</a>
  <a href="contact.html">Contact Us</a>
</nav>
<div class="container">
  <h2>Reach Out to Us</h2>
  <p><strong>Address:</strong>Sivalingam nagar Town extension Mayiladuthurai </p>
  <p><strong>Phone:</strong>9363970274</p>
  <p><strong>Email:</strong> theb&i's@gmail.com</p>
</div>
<footer>
  <p>Website designed by HARI KRISHNAN</p>
</footer>
</body>
</html>

```
contact.css
```
body {
  font-family: sans-serif;
  background-color: #f2f2f2;
  margin: 0;
}

header, footer {
  background-color: #8B0000;
  color: white;
  text-align: center;
  padding: 20px;
}

nav {
  background-color: #eee;
  text-align: center;
  padding: 10px;
}

nav a {
  margin: 0 15px;
  text-decoration: none;
  color: #8B0000;
}

.container {
  padding: 30px;
  background-color: white;
  margin: 20px;
  border-radius: 8px;
}
```

# OUTPUT:
![alt text](<Screenshot 2025-05-11 000954.png>)

![alt text](<Screenshot 2025-05-11 001006.png>)

![alt text](<Screenshot 2025-05-11 001017.png>)

![alt text](<Screenshot 2025-05-11 001042.png>)

![alt text](<Screenshot 2025-05-11 001050.png>)

![alt text](<Screenshot 2025-05-11 001102.png>)
# RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
