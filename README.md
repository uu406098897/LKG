<!DOCTYPE html>
<html lang="zh-CN">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>中国金隆之窗</title>
    <link rel="stylesheet" href="style.css">
    <!-- 引入外部CSS文件 -->
</head>

<body>
    <div class="container">
        <header>
            <h1>中国金隆之窗</h1>
            <nav>
                <ul>
                    <li><a href="#">首页</a></li>
                    <li><a href="#about">关于我们</a></li>
                    <li><a href="#products">产品中心</a></li>
                    <li><a href="#news">新闻动态</a></li>
                    <li><a href="#contact">联系我们</a></li>
                </ul>
            </nav>
        </header>

        <main>
            <section class="module" id="about">
                <h2>关于我们</h2>
                <div class="about-content">
                    <img src="images/about.jpg" alt="公司图片" class="about-image">
                    <p>
                        中国金隆之窗是一家专注于金融科技领域的创新型企业。我们致力于为客户提供高效、安全、便捷的金融解决方案，涵盖投资理财、资产管理、风险控制等多个方面。我们的团队由一群经验丰富的金融专家和技术精英组成，不断探索金融科技的前沿，为客户创造更大的价值。
                    </p>
                </div>
            </section>

            <section class="module" id="products">
                <h2>产品中心</h2>
                <div class="products-grid">
                    <div class="product-item">
                        <img src="images/product1.jpg" alt="产品1">
                        <h3>智能投顾</h3>
                        <p>基于大数据和人工智能的个性化投资组合推荐。</p>
                    </div>
                    <div class="product-item">
                        <img src="images/product2.jpg" alt="产品2">
                        <h3>量化交易平台</h3>
                        <p>为专业投资者提供高效、稳定的量化交易工具。</p>
                    </div>
                    <div class="product-item">
                        <img src="images/product3.jpg" alt="产品3">
                        <h3>风险管理系统</h3>
                        <p>全方位的风险监测、评估和预警，保障资产安全。</p>
                    </div>
                    <div class="product-item">
                        <img src="images/product4.jpg" alt="产品4">
                        <h3>区块链金融应用</h3>
                        <p>探索区块链技术在金融领域的创新应用。</p>
                    </div>
                </div>
            </section>

            <section class="module" id="news">
                <h2>新闻动态</h2>
                <div class="news-container">
                    <div class="news-item">
                        <img src="images/news1.jpg" alt="新闻1">
                        <h3>公司荣获“年度金融科技创新奖”</h3>
                        <p>在近日举行的金融科技峰会上，中国金隆之窗凭借其卓越的创新能力和产品表现，荣获“年度金融科技创新奖”。</p>
                        <a href="#">阅读更多</a>
                    </div>
                    <div class="news-item">
                        <img src="images/news2.jpg" alt="新闻2">
                        <h3>与知名投资机构达成战略合作</h3>
                        <p>中国金隆之窗宣布与知名投资机构达成战略合作，共同推动金融科技领域的创新发展。</p>
                        <a href="#">阅读更多</a>
                    </div>
                </div>
            </section>
             <section class="module" id="hot-news">
                <h2>百度热搜</h2>
                <ul id="baidu-hot-news"></ul>
            </section>
            <section class="module" id="weather">
                <h2>主要城市天气</h2>
                <div id="weather-container"></div>
            </section>

            <section class="module" id="contact">
                <h2>联系我们</h2>
                <div class="contact-info">
                    <p>地址：浙江省杭州市西湖区...</p>
                    <p>电话：...</p>
                    <p>邮箱：...</p>
                </div>
                <form class="contact-form">
                    <input type="text" placeholder="您的姓名">
                    <input type="email" placeholder="您的邮箱">
                    <textarea placeholder="您的留言"></textarea>
                    <button type="submit">提交</button>
                </form>
            </section>
        </main>

        <footer>
            <p>&copy; 2024 中国金隆之窗. All rights reserved.</p>
        </footer>
    </div>

    <script src="script.js"></script>
    <!-- 引入外部JS文件 -->
</body>

</html>
/* 全局样式 */
body {
    font-family: "微软雅黑", sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f5f5f5;
    color: #333;
}

.container {
    width: 90%;
    max-width: 1400px;
    margin: 0 auto;
}

/* 头部样式 */
header {
    background: linear-gradient(to right, #ff9900, #ffcc66);
    color: white;
    padding: 20px 0;
    text-align: center;
}

header h1 {
    font-size: 3em;
    margin: 0;
}

nav ul {
    list-style: none;
    padding: 0;
    margin: 10px 0 0 0;
}

nav ul li {
    display: inline;
    margin: 0 15px;
}

nav ul li a {
    color: white;
    text-decoration: none;
    font-size: 1.2em;
}

/* 模块样式 */
.module {
    padding: 20px;
    margin-bottom: 20px;
    background-color: white;
    border-radius: 5px;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
}

.module h2 {
    font-size: 1.8em;
    margin-bottom: 10px;
    border-bottom: 2px solid #ff9900;
    padding-bottom: 5px;
}

/* 关于我们 */
.about-content {
    display: flex;
    align-items: center;
}

.about-image {
    width: 300px;
    margin-right: 20px;
    border-radius: 5px;
}

/* 产品中心 */
.products-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 20px;
}

.product-item {
    text-align: center;
    padding: 10px;
    border: 1px solid #ddd;
    border-radius: 5px;
}

.product-item img {
    width: 100%;
    max-height: 150px;
    object-fit: cover;
    border-radius: 5px;
}

/* 新闻动态 */
.news-container {
    display: flex;
    justify-content: space-between;
}

.news-item {
    width: 48%;
    /* 留一点空间给间距 */
    padding: 10px;
    border: 1px solid #ddd;
    border-radius: 5px;
}

.news-item img {
    width: 100%;
    max-height: 200px;
    object-fit: cover;
    border-radius: 5px;
}

/* 联系我们 */
.contact-info {
    margin-bottom: 20px;
}

.contact
