<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>中国金隆之窗</title>
    <style>
        /* 基础样式 */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Microsoft YaHei', sans-serif;
        }

        /* 天气预报栏 */
        .weather-bar {
            background: #004a87;
            color: white;
            padding: 8px 0;
            overflow: hidden;
        }

        .weather-scroll {
            white-space: nowrap;
            animation: scroll 30s linear infinite;
        }

        @keyframes scroll {
            0% { transform: translateX(100%); }
            100% { transform: translateX(-100%); }
        }

        /* 头部样式 */
        header {
            background: #fff;
            padding: 20px 0;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }

        .logo {
            font-size: 28px;
            color: #004a87;
            font-weight: bold;
            text-align: center;
        }

        /* 导航菜单 */
        nav {
            background: #004a87;
            padding: 15px 0;
        }

        nav ul {
            display: flex;
            justify-content: center;
            list-style: none;
        }

        nav a {
            color: white;
            text-decoration: none;
            padding: 0 20px;
            transition: color 0.3s;
        }

        nav a:hover {
            color: #ffd700;
        }

        /* 轮播图 */
        .carousel {
            height: 400px;
            background: #f5f5f5;
            position: relative;
            overflow: hidden;
        }

        .carousel-item {
            position: absolute;
            width: 100%;
            height: 100%;
            opacity: 0;
            transition: opacity 1s;
        }

        .carousel-item.active {
            opacity: 1;
        }

        /* 内容区块 */
        .section {
            padding: 50px 20px;
        }

        .section-title {
            text-align: center;
            margin-bottom: 30px;
            color: #004a87;
        }

        /* 产品展示 */
        .products {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
            max-width: 1200px;
            margin: 0 auto;
        }

        .product-card {
            border: 1px solid #ddd;
            padding: 20px;
            border-radius: 5px;
            text-align: center;
        }

        /* 底部样式 */
        footer {
            background: #333;
            color: white;
            padding: 30px 20px;
            text-align: center;
        }
    </style>
</head>
<body>
    <!-- 天气预报 -->
    <div class="weather-bar">
        <div class="weather-scroll" id="weatherInfo">
            正在获取天气信息...
        </div>
    </div>

    <!-- 网站头部 -->
    <header>
        <div class="logo">中国金隆之窗</div>
    </header>

    <!-- 导航菜单 -->
    <nav>
        <ul>
            <li><a href="#home">首页</a></li>
            <li><a href="#about">关于我们</a></li>
            <li><a href="#products">产品中心</a></li>
            <li><a href="#news">新闻动态</a></li>
            <li><a href="#contact">联系我们</a></li>
        </ul>
    </nav>

    <!-- 轮播图 -->
    <div class="carousel">
        <div class="carousel-item active" style="background: url('placeholder1.jpg') center/cover;"></div>
        <div class="carousel-item" style="background: url('placeholder2.jpg') center/cover;"></div>
        <div class="carousel-item" style="background: url('placeholder3.jpg') center/cover;"></div>
    </div>

    <!-- 产品展示 -->
    <section class="section">
        <h2 class="section-title">产品中心</h2>
        <div class="products">
            <div class="product-card">
                <h3>产品分类一</h3>
                <p>产品描述内容...</p>
            </div>
            <div class="product-card">
                <h3>产品分类二</h3>
                <p>产品描述内容...</p>
            </div>
            <div class="product-card">
                <h3>产品分类三</h3>
                <p>产品描述内容...</p>
            </div>
        </div>
    </section>

    <!-- 网站底部 -->
    <footer>
        <p>© 2023 中国金隆之窗 版权所有</p>
        <p>地址：XXX省XXX市XXX区XXX路XX号</p>
    </footer>

    <script>
        // 轮播图逻辑
        let currentSlide = 0;
        const slides = document.querySelectorAll('.carousel-item');
        
        function nextSlide() {
            slides[currentSlide].classList.remove('active');
            currentSlide = (currentSlide + 1) % slides.length;
            slides[currentSlide].classList.add('active');
        }
        setInterval(nextSlide, 5000);

        // 天气预报功能（示例数据，需要替换真实API）
        const weatherData = [
            "北京：晴 25℃/18℃",
            "上海：多云 28℃/22℃",
            "广州：阵雨 30℃/25℃",
            "深圳：晴 31℃/26℃"
        ];
        
        const weatherInfo = document.getElementById('weatherInfo');
        weatherInfo.textContent = weatherData.join('　|　') + '　';
    </script>
</body>
</html>
