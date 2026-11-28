
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Sri Velavan Bakes</title>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Arial, sans-serif;
}

body {
    background: #fff5e6;
    color: #333;
}

header {
    background: linear-gradient(120deg, #ff512f, #ff9800);
    color: white;
    text-align: center;
    padding: 35px 15px;
}

header h1 {
    font-size: 38px;
}

header p {
    margin-top: 10px;
    font-size: 17px;
}

nav {
    background: #5b8c36;
    padding: 15px;
    text-align: center;
}

nav a {
    color: white;
    text-decoration: none;
    margin: 15px;
    font-weight: bold;
}

.hero {
    text-align: center;
    padding: 45px 15px;
    background: linear-gradient(120deg, #ffe082, #ffccbc);
}

.hero h2 {
    color: #d84315;
    font-size: 30px;
}

.hero p {
    margin: 15px;
    font-size: 18px;
}

.products {
    padding: 35px 20px;
    text-align: center;
}

.products h2 {
    color: #e65100;
    font-size: 30px;
    margin-bottom: 25px;
}

.container {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(210px, 1fr));
    gap: 22px;
    max-width: 1100px;
    margin: auto;
}

.card {
    background: white;
    padding: 25px 15px;
    border-radius: 15px;
    box-shadow: 0 4px 12px #0002;
    border-bottom: 5px solid #ff9800;
    transition: 0.3s;
}

.card:hover {
    transform: translateY(-7px);
}

.card h3 {
    color: #e65100;
    font-size: 21px;
    margin-bottom: 12px;
}

.price {
    color: #228b22;
    font-size: 20px;
    font-weight: bold;
    margin: 12px;
}

.order {
    display: inline-block;
    background: #25d366;
    color: white;
    padding: 11px 20px;
    text-decoration: none;
    border-radius: 25px;
    font-weight: bold;
}

.order:hover {
    background: #128c45;
}

.about {
    background: #dcedc8;
    text-align: center;
    padding: 35px 20px;
}

.about h2 {
    color: #33691e;
    margin-bottom: 15px;
}

.contact {
    text-align: center;
    padding: 35px 15px;
    background: #ffe0b2;
}

.contact h2 {
    color: #e65100;
    margin-bottom: 15px;
}

footer {
    background: #333;
    color: white;
    text-align: center;
    padding: 20px;
}
</style>
</head>

<body>

<header>
    <h1>🍰 SRI VELAVAN BAKES 🍰</h1>
    <p>Fresh Taste • Sweet Moments • Happy Customers</p>
</header>

<nav>
    <a href="#home">Home</a>
    <a href="#products">Products</a>
    <a href="#about">About</a>
    <a href="#contact">Contact</a>
</nav>

<section class="hero" id="home">
    <h2>Welcome to Sri Velavan Bakes!</h2>
    <p>Delicious Bakery Products at Best Prices!</p>
    <p>Freshness and Happiness in Every Bite ❤️</p>
    <a href="#products" class="order">Explore Products</a>
</section>

<section class="products" id="products">
    <h2>🛍️ Our Products & Sales</h2>

    <div class="container">

        <div class="card">
            <h3>🎂 Birthday Cake</h3>
            <p>Fresh and Delicious Cake</p>
            <div class="price">₹450</div>
            <a class="order" href="#" onclick="order('Birthday Cake',450)">WhatsApp Order</a>
        </div>

        <div class="card">
            <h3>🧁 Cup Cake</h3>
            <p>Soft and Sweet Cup Cakes</p>
            <div class="price">₹50</div>
            <a class="order" href="#" onclick="order('Cup Cake',50)">WhatsApp Order</a>
        </div>

        <div class="card">
            <h3>🍕 Pizza</h3>
            <p>Cheesy and Tasty Pizza</p>
            <div class="price">₹120</div>
            <a class="order" href="#" onclick="order('Pizza',120)">WhatsApp Order</a>
        </div>

        <div class="card">
            <h3>🍔 Burger</h3>
            <p>Fresh and Crispy Burger</p>
            <div class="price">₹80</div>
            <a class="order" href="#" onclick="order('Burger',80)">WhatsApp Order</a>
        </div>

        <div class="card">
            <h3>🥐 Puffs</h3>
            <p>Hot and Crispy Puffs</p>
            <div class="price">₹20</div>
            <a class="order" href="#" onclick="order('Puffs',20)">WhatsApp Order</a>
        </div>

        <div class="card">
            <h3>🍩 Donuts</h3>
            <p>Sweet and Delicious Donuts</p>
            <div class="price">₹60</div>
            <a class="order" href="#" onclick="order('Donuts',60)">WhatsApp Order</a>
        </div>

    </div>
</section>

<section class="about" id="about">
    <h2>About Sri Velavan Bakes</h2>
    <p>
        Sri Velavan Bakes offers delicious bakery products
        with great taste and quality.
        Visit us and enjoy every bite!
    </p>
</section>

<section class="contact" id="contact">
    <h2>📞 Contact Us</h2>
    <p>For orders and enquiries, contact us on WhatsApp.</p>
    <br>
    <a class="order" href="https://wa.me/91XXXXXXXXXX">
        Order Now on WhatsApp
    </a>
</section>

<footer>
    <p>© 2026 Sri Velavan Bakes | All Rights Reserved</p>
    <p>Thank You! Visit Again ❤️</p>
</footer>

<script>
const whatsappNumber = "91XXXXXXXXXX";

function order(product, price) {
    const message = `Hello Sri Velavan Bakes! I want to order ${product}. Price: ₹${price}.`;
    const url = `https://wa.me/${whatsappNumber}?text=${encodeURIComponent(message)}`;
    window.open(url, "_blank");
}
</script>

</body>
</html>
