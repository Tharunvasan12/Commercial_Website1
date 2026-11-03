# Ex02 Commercial Website
## Date:31/10/2026

## AIM
To create a commercial website using CSS Flexbox.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5
Include social media links at the footer with copyright information.

### STEP 6
Define global styles for fonts, colors, and layout.

### STEP 7
Style the header, navigation bar, and sections.

### STEP 8
Use Flexbox for layout design.

### STEP 9
Add hover effects and transitions for interactivity.

### STEP 10
Add Images and Media.

### STEP 11
Use optimized images for a professional look.

### STEP 12
Open the HTML file in a browser to check layout and functionality.

### STEP 13
Fix styling issues and refine content placement.

### STEP 14
Deploy the website.

### STEP 15
Upload to GitHub Pages for free hosting.

## PROGRAM
index.html
```

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>NovaStore - Online Shopping</title>
    <link rel="stylesheet" href="style.css">
</head>

<body>

    <!-- Navigation Bar -->
    <header>
        <nav class="navbar">
            <h1 class="logo">Nova<span>Store</span></h1>

            <div class="nav-links">
                <a href="#home">Home</a>
                <a href="#categories">Categories</a>
                <a href="#products">Products</a>
                <a href="#about">About</a>
                <a href="#contact">Contact</a>
            </div>

            <a href="#products" class="cart">Shop Now</a>
        </nav>
    </header>

    <!-- Hero Section -->
    <section class="hero" id="home">

        <div class="hero-content">
            <p class="tagline">WELCOME TO NOVASTORE</p>

            <h2>Discover the Latest<br>Trends & Technology</h2>

            <p>
                Explore quality products at amazing prices.
                Find everything you need in one place.
            </p>

            <a href="#products" class="btn">Explore Products</a>
        </div>

        <div class="hero-image">
            <img src="https://images.unsplash.com/photo-1498049794561-7780e7231661?w=700"
                 alt="Electronic products">
        </div>

    </section>

    <!-- Categories Section -->
    <section class="categories" id="categories">

        <h2>Shop By Category</h2>

        <div class="category-container">

            <div class="category-box">
                <h3>Electronics</h3>
                <p>Latest gadgets and devices</p>
            </div>

            <div class="category-box">
                <h3>Fashion</h3>
                <p>Discover your style</p>
            </div>

            <div class="category-box">
                <h3>Accessories</h3>
                <p>Complete your look</p>
            </div>

            <div class="category-box">
                <h3>Home Essentials</h3>
                <p>Upgrade your lifestyle</p>
            </div>

        </div>

    </section>

    <!-- Products Section -->
    <section class="products" id="products">

        <h2>Featured Products</h2>

        <div class="product-container">

            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1505740420928-5e560c06d30e?w=500"
                     alt="Headphones">

                <h3>Wireless Headphones</h3>
                <p>High quality wireless audio experience.</p>
                <h4>₹2,499</h4>
                <button>Add to Cart</button>
            </div>

            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1523275335684-37898b6baf30?w=500"
                     alt="Smart Watch">

                <h3>Smart Watch</h3>
                <p>Track your fitness and daily activities.</p>
                <h4>₹3,499</h4>
                <button>Add to Cart</button>
            </div>

            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1503602642458-232111445657?w=500"
                     alt="Chair">

                <h3>Modern Chair</h3>
                <p>Comfortable and stylish furniture.</p>
                <h4>₹4,999</h4>
                <button>Add to Cart</button>
            </div>

            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1526170375885-4d8ecf77b99f?w=500"
                     alt="Camera">

                <h3>Digital Camera</h3>
                <p>Capture your favourite moments.</p>
                <h4>₹8,999</h4>
                <button>Add to Cart</button>
            </div>

        </div>

    </section>

    <!-- About Section -->
    <section class="about" id="about">

        <h2>About NovaStore</h2>

        <p>
            NovaStore is an online shopping destination offering
            quality products across multiple categories.
            Our mission is to provide a convenient and enjoyable
            shopping experience for every customer.
        </p>

    </section>

    <!-- Contact Section -->
    <section class="contact" id="contact">

        <h2>Contact Us</h2>

        <p>Email: support@novastore.com</p>
        <p>Phone: +91 98765 43210</p>
        <p>Location: Chennai, India</p>

    </section>

    <!-- Footer -->
    <footer>

        <h3>NovaStore</h3>

        <p>Quality Products. Better Shopping Experience.</p>

        <hr>

        <p>Designed by: Tharunish Vasan</p>

        <p>Register Number: YOUR REGISTER NUMBER</p>

        <p>Copyright &copy; 2026 NovaStore. All Rights Reserved.</p>

    </footer>

</body>
</html>
```
style.css
```

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Arial, sans-serif;
    scroll-behavior: smooth;
}

body {
    background-color: #f5f6fa;
    color: #222;
}

/* Navigation Bar */

header {
    background-color: #111827;
    padding: 20px 8%;
}

.navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: 20px;
}

.logo {
    color: white;
    font-size: 28px;
}

.logo span {
    color: #ff9f1c;
}

.nav-links {
    display: flex;
    gap: 25px;
    flex-wrap: wrap;
}

.nav-links a {
    text-decoration: none;
    color: white;
    font-size: 15px;
}

.nav-links a:hover {
    color: #ff9f1c;
}

.cart {
    background-color: #ff9f1c;
    color: #111827;
    padding: 10px 20px;
    border-radius: 5px;
    text-decoration: none;
    font-weight: bold;
}

/* Hero Section */

.hero {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 70px 8%;
    gap: 40px;
    background-color: #e9eef7;
    flex-wrap: wrap;
}

.hero-content {
    flex: 1;
    min-width: 280px;
}

.tagline {
    color: #e58a00;
    font-weight: bold;
    margin-bottom: 15px;
}

.hero-content h2 {
    font-size: 42px;
    margin-bottom: 20px;
    color: #111827;
}

.hero-content p {
    line-height: 1.7;
    margin-bottom: 25px;
}

.btn {
    display: inline-block;
    background-color: #ff9f1c;
    color: #111827;
    padding: 13px 25px;
    text-decoration: none;
    border-radius: 5px;
    font-weight: bold;
}

.hero-image {
    flex: 1;
    min-width: 280px;
}

.hero-image img {
    width: 100%;
    max-height: 350px;
    object-fit: cover;
    border-radius: 15px;
}

/* Categories Section */

.categories {
    padding: 60px 8%;
    text-align: center;
}

.categories h2,
.products h2,
.about h2,
.contact h2 {
    font-size: 30px;
    margin-bottom: 35px;
}

.category-container {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 20px;
}

.category-box {
    flex: 1 1 200px;
    padding: 30px 15px;
    background-color: white;
    border-radius: 10px;
    box-shadow: 0 3px 12px #00000010;
}

.category-box h3 {
    margin-bottom: 12px;
    color: #e58a00;
}

/* Products Section */

.products {
    padding: 60px 8%;
    background-color: #e9eef7;
    text-align: center;
}

.product-container {
    display: flex;
    justify-content: center;
    align-items: stretch;
    flex-wrap: wrap;
    gap: 25px;
}

.product-card {
    flex: 1 1 220px;
    max-width: 280px;
    background-color: white;
    padding: 18px;
    border-radius: 12px;
    box-shadow: 0 3px 12px #00000015;
    text-align: center;
    transition: 0.3s;
}

.product-card:hover {
    transform: translateY(-8px);
}

.product-card img {
    width: 100%;
    height: 180px;
    object-fit: cover;
    border-radius: 8px;
}

.product-card h3 {
    margin: 15px 0 10px;
}

.product-card p {
    color: #666;
    line-height: 1.5;
    margin-bottom: 12px;
}

.product-card h4 {
    color: #e58a00;
    font-size: 20px;
    margin-bottom: 15px;
}

.product-card button {
    background-color: #111827;
    color: white;
    border: none;
    padding: 11px 20px;
    border-radius: 5px;
    cursor: pointer;
}

.product-card button:hover {
    background-color: #ff9f1c;
    color: #111827;
}

/* About Section */

.about {
    padding: 60px 15%;
    text-align: center;
}

.about p {
    line-height: 1.8;
    color: #555;
}

/* Contact Section */

.contact {
    background-color: #e9eef7;
    padding: 60px 8%;
    text-align: center;
}

.contact p {
    margin: 12px 0;
}

/* Footer */

footer {
    background-color: #111827;
    color: white;
    text-align: center;
    padding: 30px 15px;
    line-height: 2;
}

footer h3 {
    color: #ff9f1c;
    font-size: 25px;
}

footer hr {
    margin: 15px auto;
    max-width: 500px;
}

/* Responsive Design */

@media (max-width: 768px) {

    .navbar {
        flex-direction: column;
    }

    .nav-links {
        justify-content: center;
    }

    .hero {
        flex-direction: column;
        text-align: center;
    }

    .hero-content h2 {
        font-size: 32px;
    }

    .hero-image {
        width: 100%;
    }

    .product-card {
        flex: 1 1 250px;
    }

}

@media (max-width: 480px) {

    .nav-links {
        gap: 12px;
    }

    .nav-links a {
        font-size: 13px;
    }

    .hero-content h2 {
        font-size: 27px;
    }

    .categories h2,
    .products h2,
    .about h2,
    .contact h2 {
        font-size: 25px;
    }

}
```
## OUTPUT


## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.