<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>中国金隆之窗</title>
    <style>
        body {
            margin: 0;
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
        }
        header {
            background: linear-gradient(to right, #ff9900, #ff6600);
            color: white;
            padding: 20px;
            text-align: center;
            font-size: 2em;
            font-weight: bold;
        }
        .container {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-around;
            padding: 20px;
        }
        .module {
            background-color: white;
            border-radius: 8px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
            width: 30%;
            margin: 10px;
            padding: 20px;
            text-align: center;
        }
        .module h2 {
            margin-top: 0;
        }
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 10px;
            position: relative;
            bottom: 0;
            width: 100%;
        }
        .scroll-container {
            overflow: hidden;
            height: 100px;
            margin: 20px auto;
            width: 80%;
            border: 1px solid #ccc;
            background-color: white;
        }
        .scroll-content {
            animation: scroll 10s linear infinite;
        }
        @keyframes scroll {
            0% { transform: translateY(0); }
            100% { transform: translateY(-100%); }
        }
        .weather-container {
            margin: 20px auto;
            width: 80%;
            background-color: white;
            border: 1px solid #ccc;
            padding: 10px;
            text-align: center;
        }
    </style>
</head>
<body>
    <header>中国金隆之窗</header>
    <div class="container">
        <!-- 模块1 -->
        <div class="module">
            <h2>关于我们</h2>
            <p>中国金隆之窗是一个致力于分享信息、传播文化的平台。</p>
        </div>
        <!-- 模块2 -->
        <div class="module">
            <h2>最新动态</h2>
            <p>我们每天更新最新的新闻和资讯，关注我们获取第一手消息。</p>
        </div>
        <!-- 模块3 -->
        <div class="module">
            <h2>热门话题</h2>
            <p>讨论当下最热门的话题，与志同道合的朋友一起交流。</p>
        </div>
        <!-- 模块4 -->
        <div class="module">
            <h2>文化专栏</h2>
            <p>了解中国传统文化，感受历史的魅力。</p>
        </div>
        <!-- 模块5 -->
        <div class="module">
            <h2>旅游推荐</h2>
            <p>探索中国的美丽风景，规划你的下一次旅行。</p>
        </div>
        <!-- 模块6 -->
        <div class="module">
            <h2>美食天地</h2>
            <p>品尝各地特色美食，满足你的味蕾。</p>
        </div>
        <!-- 模块7 -->
        <div class="module">
            <h2>科技前沿</h2>
            <p>关注科技创新，了解未来趋势。</p>
        </div>
        <!-- 模块8 -->
        <div class="module">
            <h2>教育专区</h2>
            <p>提供学习资源，助力你的成长之路。</p>
        </div>
        <!-- 模块9 -->
        <div class="module">
            <h2>健康生活</h2>
            <p>关注健康，享受美好生活。</p>
        </div>
        <!-- 模块10 -->
        <div class="module">
            <h2>娱乐频道</h2>
            <p>分享电影、音乐、游戏等娱乐内容。</p>
        </div>
        <!-- 模块11 -->
        <div class="module">
            <h2>公益活动</h2>
            <p>参与公益事业，为社会贡献力量。</p>
        </div>
        <!-- 模块12 -->
        <div class="module">
            <h2>联系我们</h2>
            <p>有任何问题或建议，请随时联系我们。</p>
        </div>
    </div>

    <!-- 动态滚动的百度热搜 -->
    <div class="scroll-container">
        <div class="scroll-content" id="hot-news"></div>
    </div>

    <!-- 国内主要城市天气动态 -->
    <div class="weather-container" id="weather-info">
        <h2>国内主要城市天气</h2>
        <div id="weather-list"></div>
    </div>

    <footer>
        浙江省杭州市西湖区 | 联系电话：123-456-7890 | 邮箱：info@jinlong.com
    </footer>

    <script>
        // 获取百度热搜数据并显示
        async function fetchHotNews() {
            try {
                const response = await fetch('https://api.example.com/baidu-hot-search'); // 替换为实际API
                const data = await response.json();
                const newsList = data.slice(0, 10).map(item => `<p>${item.title}</p>`).join('');
                document.getElementById('hot-news').innerHTML = newsList;
            } catch (error) {
                console.error('获取百度热搜失败:', error);
            }
        }

        // 获取国内主要城市天气数据并显示
        async function fetchWeather() {
            try {
                const cities = ['北京', '上海', '广州', '深圳', '杭州', '成都'];
                const weatherList = await Promise.all(cities.map(async city => {
                    const response = await fetch(`https://api.example.com/weather?city=${city}`); // 替换为实际API
                    const data = await response.json();
                    return `<p>${city}: ${data.temperature}°C, ${data.condition}</p>`;
                }));
                document.getElementById('weather-list').innerHTML = weatherList.join('');
            } catch (error) {
                console.error('获取天气数据失败:', error);
            }
        }

        // 初始化页面
        window.onload = () => {
            fetchHotNews();
            fetchWeather();
        };
    </script>
</body>
</html>
