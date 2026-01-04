# Ex.06 Restaurant Website
## Date: 3.12.2026

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
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Savory Bistro - Contact Us</title>
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

    <div class="contact-page">
        <div class="contact-header">
            <h1>Get In Touch</h1>
            <p>We'd love to hear from you</p>
        </div>

        <div class="contact-container">
            <div class="contact-info">
                <div class="info-card">
                    <div class="info-icon">📍</div>
                    <h3>Visit Us</h3>
                    <p>123 Culinary Avenue<br>Food District, City 12345</p>
                </div>

                <div class="info-card">
                    <div class="info-icon">📞</div>
                    <h3>Call Us</h3>
                    <p>+1 (555) 123-4567<br>+1 (555) 987-6543</p>
                </div>

                <div class="info-card">
                    <div class="info-icon">✉️</div>
                    <h3>Email Us</h3>
                    <p>info@crfoods.com<br>reservations@crfoods.com</p>
                </div>

                <div class="info-card">
                    <div class="info-icon">🕒</div>
                    <h3>Opening Hours</h3>
                    <p>Mon - Fri: 11:00 AM - 10:00 PM<br>
                    Sat - Sun: 10:00 AM - 11:00 PM</p>
                </div>
            </div>

            <div class="contact-form-container">
                <h2>Send Us a Message</h2>
                <form onsubmit="handleContact(event)" class="contact-form">
                    <div class="form-row">
                        <div class="form-group">
                            <label for="name">Full Name</label>
                            <input type="text" id="name" placeholder="John Doe" required>
                        </div>

                        <div class="form-group">
                            <label for="email">Email Address</label>
                            <input type="email" id="email" placeholder="john@example.com" required>
                        </div>
                    </div>

                    <div class="form-row">
                        <div class="form-group">
                            <label for="phone">Phone Number</label>
                            <input type="tel" id="phone" placeholder="+1 (555) 123-4567">
                        </div>

                        <div class="form-group">
                            <label for="subject">Subject</label>
                            <select id="subject" required>
                                <option value="">Select a topic</option>
                                <option value="reservation">Reservation</option>
                                <option value="feedback">Feedback</option>
                                <option value="catering">Catering</option>
                                <option value="other">Other</option>
                            </select>
                        </div>
                    </div>

                    <div class="form-group">
                        <label for="message">Message</label>
                        <textarea id="message" rows="6" placeholder="Tell us how we can help you..." required></textarea>
                    </div>

                    <button type="submit" class="submit-button">Send Message</button>
                </form>
            </div>
        </div>

        <div class="map-container">
            <h2>Find Us Here</h2>
            <div class="map-placeholder">
                <div class="map-icon">🗺️</div>
                <p>Map Location</p>
            </div>
        </div>
    </div>

    <footer>
        <p>&copy; 2025 CR Foods. All rights reserved.</p>
    </footer>

    <script>
        function handleContact(e) {
            e.preventDefault();
            const name = document.getElementById('name').value;
            const email = document.getElementById('email').value;
            const subject = document.getElementById('subject').value;
            alert('Thank you for contacting us, ' + name + '! We will get back to you soon at ' + email);
        }
    </script>
</body>
</html>

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
            <li><a href="contacts.html">Contact</a></li>
            <li><a href="login.html">Login</a></li>
        </ul>
    </nav>

    <section class="hero">
        <div class="hero-content">
            <h1>CR Restaurant</h1>
            <p>Good food is the foundation of genuine happiness.</p>
            <a href="menu.html" class="cta-button">Explore Our Menu</a>
        </div>
    </section>

    <section class="features">
        <div class="feature-card">
            <div class="feature-icon">🍽️</div>
            <h3>Fresh Ingredients</h3>
            <p>Fresh from the source to your plate.</p>
        </div>
        <div class="feature-card">
            <div class="feature-icon">👨‍🍳</div>
            <h3>Expert Chefs</h3>
            <p>Where master chefs turn ingredients into art.</p>
        </div>
        <div class="feature-card">
            <div class="feature-icon">⭐</div>
            <h3>5-Star Service</h3>
            <p>Luxury begins with quality ingredients and flawless service.</p>
        </div>
    </section>

    <footer>
        <p>&copy; 2025 CR Foods. All rights reserved.</p>
    </footer>
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Savory Bistro - Login</title>
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

    <div class="login-page">
        <div class="login-container">
            <div class="login-header">
                <h1>Welcome Back</h1>
                <p>Login to your account</p>
            </div>

            <form onsubmit="handleLogin(event)">
                <div class="form-group">
                    <label for="email">Email Address</label>
                    <input type="email" id="email" placeholder="Enter your email" required>
                </div>

                <div class="form-group">
                    <label for="password">Password</label>
                    <input type="password" id="password" placeholder="Enter your password" required>
                </div>

                <button type="submit" class="login-button">Login</button>

                <div class="login-footer">
                    <p>Don't have an account? <a href="#">Sign up</a></p>
                    <p><a href="#">Forgot password?</a></p>
                </div>
            </form>
        </div>
    </div>

    <script>
        function handleLogin(e) {
            e.preventDefault();
            const email = document.getElementById('email').value;
            alert('Login functionality would be connected to backend. Email: ' + email);
        }
    </script>
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Savory Bistro - Menu</title>
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
                    <img src="img 1.jpeg">
                </div>
                <div class="menu-item-content">
                    <h3>Grilled Ribeye Steak</h3>
                    <p>Premium aged beef, perfectly grilled with herb butter and seasonal vegetables</p>
                    <div class="price">$32.99</div>
                </div>
            </div>

            <div class="menu-item">
                <div class="menu-item-image menu-item-2">
                    <img src="img 2.jpeg">
                </div>
                <div class="menu-item-content">
                    <h3>Truffle Pasta</h3>
                    <p>Handmade fettuccine with wild mushrooms, truffle oil, and parmesan cream</p>
                    <div class="price">$24.99</div>
                </div>
            </div>

            <div class="menu-item">
                <div class="menu-item-image menu-item-3">
                    <img src="img 3.jpeg">
                </div>
                <div class="menu-item-content">
                    <h3>Lobster Thermidor</h3>
                    <p>Fresh Atlantic lobster in creamy cognac sauce, served with asparagus</p>
                    <div class="price">$45.99</div>
                </div>
            </div>

            <div class="menu-item">
                <div class="menu-item-image menu-item-4">
                    <img src="img 4.jpeg">
                </div>
                <div class="menu-item-content">
                    <h3>Chef's Sushi Platter</h3>
                    <p>Assorted premium sushi and sashimi with wasabi and pickled ginger</p>
                    <div class="price">$38.99</div>
                </div>
            </div>

            <div class="menu-item">
                <div class="menu-item-image menu-item-5">
                    <img src="img 5.jpeg">
                </div>
                <div class="menu-item-content">
                    <h3>Chocolate Lava Cake</h3>
                    <p>Warm chocolate cake with molten center, vanilla ice cream and berries</p>
                    <div class="price">$12.99</div>
                </div>
            </div>

            <div class="menu-item">
                <div class="menu-item-image menu-item-6">
                    <img src="img 6.jpeg">
                </div>
                <div class="menu-item-content">
                    <h3>Wine Selection</h3>
                    <p>Premium wines from around the world, perfectly paired with your meal</p>
                    <div class="price">$15-65</div>
                </div>
            </div>
        </div>
    </div>

    <footer>
        <p>&copy; 2025 CR Foods. All rights reserved.</p>
    </footer>
</body>
</html>
```
## OUTPUT:
<img width="1177" height="769" alt="Screenshot 2026-01-04 225727" src="https://github.com/user-attachments/assets/96ac3007-f3a9-4691-9fd3-049b63249aff" />

<img width="1919" height="907" alt="image" src="https://github.com/user-attachments/assets/e766384c-2a02-465c-9fb9-936e938e76a8" />

<img width="1900" height="911" alt="image" src="https://github.com/user-attachments/assets/3312623c-70ca-4a53-91ef-4b575022250a" />

<img width="1902" height="915" alt="image" src="https://github.com/user-attachments/assets/cdce769d-e3db-46ab-a9c1-c44d5289c427" />

<img width="1894" height="913" alt="image" src="https://github.com/user-attachments/assets/2c454fc6-7d5f-43c1-a608-8730735d938e" />


## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
