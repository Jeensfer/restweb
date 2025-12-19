# Ex.06 Restaurant Website
## Date: 17-12-2025

## AIM:
To develop a static Restaurant website to display the food items and services provided by them.

## DESIGN STEPS:

### Step 1:
Requirement collection.

### Step 2:
Creating the layout using HTML and CSS.

### Step 3:
Updating the sample content.

### Step 4:
Choose the appropriate style and color scheme.

### Step 5:
Validate the layout in various browsers.

### Step 6:
Validate the HTML code.

### Step 7:
Publish the website in the given URL.

## PROGRAM:
```
Index.Html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CR Restaurant - Home</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <nav>
        <ul>
            <li><a href="index.html">Home</a></li>
            <li><a href="menu.html">Menu</a></li>
            <li><a href="contact.html">Contact</a></li>
            <li><a href="login.html">Login</a></li>
        </ul>
    </nav>

    <section class="hero">
        <div class="hero-content">
            <h1>CR Restaurant</h1>
            <p>Delicious food made just for you</p>
            <a href="menu.html" class="cta-button">See Our Menu</a>
        </div>
    </section>

    <section class="features">
        <div class="feature-card">
            <div class="feature-icon">🍽️</div>
            <h3>Fresh Ingredients</h3>
            <p>We use fresh, local ingredients to make tasty dishes.</p>
        </div>
        <div class="feature-card">
            <div class="feature-icon">👨‍🍳</div>
            <h3>Skilled Chefs</h3>
            <p>Our chefs have years of experience and cook with care.</p>
        </div>
        <div class="feature-card">
            <div class="feature-icon">⭐</div>
            <h3>Great Service</h3>
            <p>Our staff makes sure you enjoy your meal from start to finish.</p>
        </div>
    </section>

    <footer>
        <p>&copy; 2025 CR Foods. All rights reserved.</p>
    </footer>
    <script src="darkMode.js"></script>

</body>
</html>


Login.Html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Food4U - Member Login</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <nav>
        <ul>
            <li><a href="index.html">Home</a></li>
            <li><a href="menu.html">Our Menu</a></li>
            <li><a href="contact.html">Reach Us</a></li>
            <li><a href="login.html">Member Login</a></li>
        </ul>
    </nav>

    <div class="login-page">
        <div class="login-container">
            <div class="login-header">
                <h1>Welcome to Food4U</h1>
                <p>Sign in to enjoy exclusive dining offers</p>
            </div>

            <form onsubmit="handleLogin(event)">
                <div class="form-group">
                    <label for="email">Registered Email</label>
                    <input type="email" id="email" placeholder="you@example.com" required>
                </div>

                <div class="form-group">
                    <label for="password">Account Password</label>
                    <input type="password" id="password" placeholder="Enter your password" required>
                </div>

                <button type="submit" class="login-button">Access My Account</button>

                <div class="login-footer">
                    <p>New to Food4U? <a href="#">Create an account</a></p>
                    <p><a href="#">Forgot your password?</a></p>
                </div>
            </form>
        </div>
    </div>

    <script>
        function handleLogin(e) {
            e.preventDefault();
            const email = document.getElementById('email').value;
            alert('Member login will be connected to the Food4U system. Email: ' + email);
        }
    </script>
    <script src="darkMode.js"></script>

</body>
</html>


Menu.Html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Food4U - Menu</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <nav>
        <ul>
            <li><a href="index.html">Home</a></li>
            <li><a href="menu.html">Menu</a></li>
            <li><a href="contact.html">Contact</a></li>
            <li><a href="login.html">Login</a></li>
        </ul>
    </nav>

    <div class="menu-page">
        <div class="menu-header">
            <h1>Our Signature Dishes</h1>
            <p>Crafted with passion, served with love</p>
        </div>

        <div class="menu-grid">
            <div class="menu-item">
                <div class="menu-item-image">
                    <img src="Sushi.jpg">
                </div>
                <div class="menu-item-content">
                    <h3>Sushi</h3>
                    <p>Vinegared rice with raw fish, seafood, or vegetables.</p>
                    <div class="price">$18.99</div>
                </div>
            </div>

            <div class="menu-item">
                <div class="menu-item-image menu-item-2">
                    <img src="Ramen.jpg">
                </div>
                <div class="menu-item-content">
                    <h3>Ramen</h3>
                    <p>Noodle soup with broth, meat, and veggies.</p>
                    <div class="price">$12.99</div>
                </div>
            </div>

            <div class="menu-item">
                <div class="menu-item-image menu-item-3">
                    <img src="Tempura.jpg">
                </div>
                <div class="menu-item-content">
                    <h3>Tempura</h3>
                    <p>Lightly battered and deep-fried seafood or vegetables.</p>
                    <div class="price">$14.99</div>
                </div>
            </div>

            <div class="menu-item">
                <div class="menu-item-image menu-item-4">
                    <img src="Oko.jpg">
                </div>
                <div class="menu-item-content">
                    <h3>Okonomiyaki</h3>
                    <p>Savory pancake with cabbage, meat/seafood, and sauce.</p>
                    <div class="price">$11.99</div>
                </div>
            </div>

            <div class="menu-item">
                <div class="menu-item-image menu-item-5">
                    <img src="Ta.png">
                </div>
                <div class="menu-item-content">
                    <h3>Takoyaki</h3>
                    <p>Ball-shaped snack filled with octopus, tempura bits, and green onion.</p>
                    <div class="price">$9.99</div>
                </div>
            </div>

            <div class="menu-item">
                <div class="menu-item-image menu-item-6">
                    <img src="Miso.png">
                </div>
                <div class="menu-item-content">
                    <h3>Miso Soup</h3>
                    <p>Traditional soup with miso paste, tofu, and seaweed.</p>
                    <div class="price">$6.99</div>
                </div>
            </div>
        </div>
    </div>

    <footer>
        <p>&copy; 2025 Food4U. All rights reserved.</p>
    </footer>
    <script src="darkMode.js"></script>

</body>
</html>


Contact.Html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Contact Us</title>
  <style>
    * { box-sizing: border-box; margin: 0; padding: 0; }

    body {
      font-family: 'Segoe UI', Tahoma, sans-serif;
      background: #f4f6fb;
      color: #333;
    }

    .container {
      max-width: 1100px;
      margin: 50px auto;
      padding: 20px;
    }

    h1 {
      text-align: center;
      margin-bottom: 10px;
    }

    .subtitle {
      text-align: center;
      margin-bottom: 40px;
      color: #666;
    }

    .contact-box {
      display: grid;
      grid-template-columns: 1fr 1fr;
      background: #fff;
      border-radius: 12px;
      box-shadow: 0 10px 25px rgba(0,0,0,0.08);
      overflow: hidden;
    }

    .info {
      padding: 30px;
      background: linear-gradient(135deg, #2c3e50, #34495e);
      color: #fff;
    }

    .info h2 {
      margin-bottom: 20px;
    }

    .info p {
      margin-bottom: 12px;
      font-size: 15px;
      line-height: 1.6;
    }

    .info strong {
      display: block;
      margin-bottom: 4px;
    }

    .form {
      padding: 30px;
    }

    .form h2 {
      margin-bottom: 20px;
    }

    .form-group {
      margin-bottom: 15px;
    }

    label {
      display: block;
      margin-bottom: 6px;
      font-weight: 600;
    }

    input, select, textarea {
      width: 100%;
      padding: 10px;
      border-radius: 6px;
      border: 1px solid #ccc;
      font-size: 14px;
    }

    textarea {
      resize: vertical;
      min-height: 100px;
    }

    button {
      margin-top: 10px;
      padding: 12px;
      width: 100%;
      border: none;
      border-radius: 6px;
      background: #2c3e50;
      color: #fff;
      font-size: 16px;
      cursor: pointer;
    }

    button:hover {
      background: #1f2e3a;
    }

    footer {
      margin-top: 50px;
      text-align: center;
      padding: 20px;
      background: #1f2e3a;
      color: #fff;
    }

    @media (max-width: 768px) {
      .contact-box {
        grid-template-columns: 1fr;
      }
    }
    nav {
    position: sticky;
    top: 0;
    z-index: 1000;
    background: linear-gradient(135deg, rgba(108,99,255,0.9), rgba(0,201,167,0.9));
    backdrop-filter: blur(14px);
    box-shadow: var(--shadow-md);
    padding: 1.1rem 0;
}

nav ul {
    list-style: none;
    display: flex;
    justify-content: center;
    gap: 2.8rem;
}

nav a {
    position: relative;
    color: #fff;
    text-decoration: none;
    font-size: 1.05rem;
    font-weight: 500;
    padding: 0.6rem 1.4rem;
    border-radius: 999px;
    transition: var(--transition-mid);
}

nav a::after {
    content: "";
    position: absolute;
    inset: 0;
    border-radius: inherit;
    background: rgba(255,255,255,0.25);
    opacity: 0;
    transform: scale(0.8);
    transition: var(--transition-fast);
}

nav a:hover::after {
    opacity: 1;
    transform: scale(1);
}

nav a:hover {
    transform: translateY(-3px);
}
  </style>
</head>
<body>
<nav>
        <ul>
            <li><a href="index.html">Home</a></li>
            <li><a href="menu.html">Menu</a></li>
            <li><a href="contact.html">Contact</a></li>
            <li><a href="login.html">Login</a></li>
        </ul>
    </nav>
  <div class="container">
    <h1>Contact Us</h1>
    <p class="subtitle">We’d love to hear from you</p>

    <div class="contact-box">
      <!-- Contact Info -->
      <div class="info">
        <h2>Contact Information</h2>
        <p><strong>Address</strong>123 Food Street,<br>City, 12345</p>
        <p><strong>Phone</strong>+1 555 123 4567<br>+1 555 987 6543</p>
        <p><strong>Email</strong>info@food4u.com<br>reservations@food4u.com</p>
        <p><strong>Business Hours</strong>Mon–Fri: 11:00 AM – 10:00 PM<br>Sat–Sun: 10:00 AM – 11:00 PM</p>
      </div>

      <!-- Form -->
      <div class="form">
        <h2>Send a Message</h2>
        <div class="form-group">
          <label>Full Name</label>
          <input type="text" />
        </div>
        <div class="form-group">
          <label>Email Address</label>
          <input type="email" />
        </div>
        <div class="form-group">
          <label>Phone Number</label>
          <input type="tel" />
        </div>
        <div class="form-group">
          <label>Subject</label>
          <select>
            <option>General Inquiry</option>
            <option>Reservation</option>
            <option>Feedback</option>
          </select>
        </div>
        <div class="form-group">
          <label>Message</label>
          <textarea></textarea>
        </div>
        <button>Send Message</button>
      </div>
    </div>
  </div>

  <footer>
    © 2025 Food4U. All rights reserved.
  </footer>

</body>
</html>


```
## OUTPUT:
![alt text](<Screenshot 2025-12-19 131410.png>)
![alt text](<Screenshot 2025-12-19 131425.png>)
![alt text](<Screenshot 2025-12-19 131442.png>)
![alt text](<Screenshot 2025-12-19 131501.png>)
## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
