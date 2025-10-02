<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Cửa Hàng Quần Áo</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <div class="container">
            <h1>Cửa Hàng Quần Áo</h1>
            <nav>
                <ul>
                    <li><a href="#">Trang Chủ</a></li>
                    <li><a href="#">Sản Phẩm</a></li>
                    <li><a href="#">Giỏ Hàng</a></li>
                    <li><a href="#">Liên Hệ</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <main>
        <section class="products">
            <div class="product">
                <img src="images/shirt1.jpg" alt="Áo sơ mi 1">
                <h2>Áo Sơ Mi Nam</h2>
                <p class="price">250,000 VNĐ</p>
                <button class="buy-btn">Thêm vào giỏ</button>
            </div>
            <div class="product">
                <img src="images/shirt2.jpg" alt="Áo sơ mi 2">
                <h2>Áo Sơ Mi Nữ</h2>
                <p class="price">300,000 VNĐ</p>
                <button class="buy-btn">Thêm vào giỏ</button>
            </div>
            <div class="product">
                <img src="images/pants1.jpg" alt="Quần jean 1">
                <h2>Quần Jean Nam</h2>
                <p class="price">400,000 VNĐ</p>
                <button class="buy-btn">Thêm vào giỏ</button>
            </div>
            <div class="product">
                <img src="images/pants2.jpg" alt="Quần jean 2">
                <h2>Quần Jean Nữ</h2>
                <p class="price">450,000 VNĐ</p>
                <button class="buy-btn">Thêm vào giỏ</button>
            </div>
        </section>
    </main>

    <footer>
        <p>&copy; 2025 Cửa Hàng Quần Áo. All rights reserved.</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
    background-color: #f4f4f4;
    color: #333;
}

.container {
    width: 80%;
    margin: 0 auto;
}

header {
    background-color: #333;
    color: white;
    padding: 20px 0;
}

header h1 {
    text-align: center;
    font-size: 2.5rem;
}

nav ul {
    display: flex;
    justify-content: center;
    list-style-type: none;
}

nav ul li {
    margin: 0 15px;
}

nav ul li a {
    color: white;
    text-decoration: none;
    font-size: 1.2rem;
}

nav ul li a:hover {
    text-decoration: underline;
}

main {
    padding: 50px 0;
}

.products {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
}

.product {
    background-color: white;
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    text-align: center;
    width: 22%;
    margin: 10px 0;
    transition: transform 0.3s;
}

.product img {
    max-width: 100%;
    border-radius: 8px;
}

.product h2 {
    font-size: 1.5rem;
    margin: 20px 0;
}

.product .price {
    font-size: 1.2rem;
    color: #b12704;
    margin: 10px 0;
}

.buy-btn {
    background-color: #5cb85c;
    color: white;
    padding: 10px 20px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    transition: background-color 0.3s;
}

.buy-btn:hover {
    background-color: #4cae4c;
}

.product:hover {
    transform: translateY(-10px);
}

footer {
    background-color: #333;
    color: white;
    text-align: center;
    padding: 10px 0;
    position: relative;
    width: 100%;
}
document.querySelectorAll('.buy-btn').forEach(button => {
    button.addEventListener('click', (event) => {
        const productName = event.target.parentElement.querySelector('h2').textContent;
        alert(`Sản phẩm "${productName}" đã được thêm vào giỏ hàng!`);
    });
});
