# Trunghieu.github.io
<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Cửa Hàng Online</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <div class="container">
            <h1>Cửa Hàng Online</h1>
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
                <img src="images/product1.jpg" alt="Sản phẩm 1">
                <h2>Sản phẩm 1</h2>
                <p class="price">500,000 VNĐ</p>
                <button class="buy-btn">Mua ngay</button>
            </div>
            <div class="product">
                <img src="images/product2.jpg" alt="Sản phẩm 2">
                <h2>Sản phẩm 2</h2>
                <p class="price">700,000 VNĐ</p>
                <button class="buy-btn">Mua ngay</button>
            </div>
        </section>
    </main>

    <footer>
        <p>&copy; 2025 Cửa Hàng Online. All rights reserved.</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>
document.querySelectorAll('.buy-btn').forEach(button => {
    button.addEventListener('click', () => {
        alert('Sản phẩm đã được thêm vào giỏ hàng!');
    });
});
