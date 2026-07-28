# Ex02 Commercial Website
## Date:28-07-2026

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
### HTML
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elite Store</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <!-- Header -->
    <header>
        <h1>Elite Store</h1>

        <nav>
            <a href="#home">Home</a>
            <a href="#products">Products</a>
            <a href="#about">About</a>
            <a href="#contact">Contact</a>
            <a href="#account">Account</a>
        </nav>
    </header>

    <!-- Home -->
    <section id="home" class="hero">
        <div class="hero-text">
            <h2>Welcome to Elite Store</h2>
            <p>Your One Stop Shopping Destination</p>
            <a href="#products" class="btn">Shop Now</a>
        </div>

        <div class="hero-image">
            <img src="https://images.unsplash.com/photo-1512436991641-6745cdb1723f?w=600" alt="Shopping">
        </div>
    </section>

    <!-- Products -->
    <section id="products">

        <h2 class="title">Our Products</h2>

        <div class="product-container">

            <div class="card">
                <img src="https://images.unsplash.com/photo-1523275335684-37898b6baf30?w=400" alt="">
                <h3>Smart Watch</h3>
                <p>Latest generation smart watch.</p>
                <h4>₹4,999</h4>
            </div>

            <div class="card">
                <img src="https://images.unsplash.com/photo-1542291026-7eec264c27ff?w=400" alt="">
                <h3>Running Shoes</h3>
                <p>Comfortable and stylish shoes.</p>
                <h4>₹2,999</h4>
            </div>

            <div class="card">
                <img src="https://images.unsplash.com/photo-1511707171634-5f897ff02aa9?w=400" alt="">
                <h3>Smart Phone</h3>
                <p>Powerful performance and camera.</p>
                <h4>₹29,999</h4>
            </div>

        </div>

    </section>

    <!-- About -->
    <section id="about">

        <h2 class="title">About Us</h2>

        <div class="about-box">

            <img src="https://images.unsplash.com/photo-1556740749-887f6717d7e4?w=500" alt="">

            <div>
                <p>
                    Elite Store is an online commercial website providing
                    electronics, fashion, and lifestyle products at affordable
                    prices with quality customer service.
                </p>
            </div>

        </div>

    </section>

    <!-- Contact -->
    <section id="contact">

        <h2 class="title">Contact Us</h2>

        <div class="contact-box">

            <div>
                <h3>Address</h3>
                <p>Elite Store</p>
                <p>Chennai, Tamil Nadu</p>
            </div>

            <div>
                <h3>Email</h3>
                <p>info@elitestore.com</p>
            </div>

            <div>
                <h3>Phone</h3>
                <p>+91 9876543210</p>
            </div>

        </div>

    </section>

    <!-- Account -->
    <section id="account">

        <h2 class="title">User Account</h2>

        <div class="account-box">

            <form>

                <input type="text" placeholder="Username">

                <input type="password" placeholder="Password">

                <button>Login</button>

            </form>

        </div>

    </section>

    <!-- Footer -->

    <footer>

        <p>Follow Us</p>

        <div class="social">

            <a href="#">Facebook</a>
            <a href="#">Instagram</a>
            <a href="#">Twitter</a>
            <a href="#">LinkedIn</a>

        </div>

        <p>© 2026 Elite Store. All Rights Reserved.</p>

    </footer>

</body>
</html>
```
### CSS
```
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial, Helvetica, sans-serif;
}

body{
    background:#f4f4f4;
}

/* Header */

header{
    display:flex;
    justify-content:space-between;
    align-items:center;
    background:#1f2937;
    color:white;
    padding:20px 60px;
}

nav{
    display:flex;
    gap:20px;
}

nav a{
    text-decoration:none;
    color:white;
    transition:.3s;
}

nav a:hover{
    color:#ffd700;
}

/* Hero */

.hero{
    display:flex;
    justify-content:space-around;
    align-items:center;
    padding:60px;
    background:white;
    flex-wrap:wrap;
}

.hero-text{
    flex:1;
}

.hero-text h2{
    font-size:40px;
    margin-bottom:20px;
}

.hero-text p{
    margin-bottom:25px;
    font-size:18px;
}

.btn{
    background:#1f2937;
    color:white;
    text-decoration:none;
    padding:12px 25px;
    border-radius:5px;
}

.btn:hover{
    background:#ffd700;
    color:black;
}

.hero-image{
    flex:1;
    text-align:center;
}

.hero-image img{
    width:400px;
    border-radius:10px;
}

/* Section Title */

.title{
    text-align:center;
    margin:40px 0;
    font-size:32px;
}

/* Products */

.product-container{
    display:flex;
    justify-content:center;
    gap:30px;
    flex-wrap:wrap;
    padding:20px;
}

.card{
    width:280px;
    background:white;
    border-radius:10px;
    overflow:hidden;
    text-align:center;
    box-shadow:0 0 10px gray;
    transition:.4s;
}

.card:hover{
    transform:translateY(-10px);
}

.card img{
    width:100%;
    height:220px;
    object-fit:cover;
}

.card h3{
    margin:15px;
}

.card p{
    padding:0 10px;
}

.card h4{
    margin:15px;
    color:green;
}

/* About */

.about-box{
    display:flex;
    justify-content:center;
    align-items:center;
    gap:40px;
    padding:40px;
    flex-wrap:wrap;
}

.about-box img{
    width:350px;
    border-radius:10px;
}

.about-box p{
    width:500px;
    line-height:1.8;
}

/* Contact */

.contact-box{
    display:flex;
    justify-content:space-evenly;
    background:white;
    padding:40px;
    flex-wrap:wrap;
}

.contact-box div{
    text-align:center;
}

/* Account */

.account-box{
    display:flex;
    justify-content:center;
    margin:40px;
}

form{
    display:flex;
    flex-direction:column;
    width:320px;
    gap:15px;
}

input{
    padding:12px;
    border:1px solid gray;
}

button{
    padding:12px;
    border:none;
    background:#1f2937;
    color:white;
    cursor:pointer;
    transition:.3s;
}

button:hover{
    background:#ffd700;
    color:black;
}

/* Footer */

footer{
    background:#1f2937;
    color:white;
    text-align:center;
    padding:30px;
}

.social{
    display:flex;
    justify-content:center;
    gap:20px;
    margin:20px 0;
}

.social a{
    color:white;
    text-decoration:none;
}

.social a:hover{
    color:#ffd700;
}
```


## OUTPUT

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/68484b59-9b40-4dea-9493-ee473a37c1c4" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/363103e5-ec13-4a5a-aad6-4d5c314c2c43" />


## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
