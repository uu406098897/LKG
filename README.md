<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>中国金隆之窗</title>
    <style>
        body {
            font-family: "微软雅黑", sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f5f5f5;
        }

        .container {
            width: 90%; /* 宽页面 */
            max-width: 1400px; /* 最大宽度限制 */
            margin: 0 auto;
            overflow: hidden; /* 清除浮动 */
        }

        header {
            background: linear-gradient(to right, #ff9900, #ffcc66); /* 橘色渐变 */
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
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1>中国金隆之窗</h1>
            <nav>
                <ul>
                    <li><a href="#">首页</a></li>
                    <li><a href="#">今日动态</a></li>
                    <li><a href="#">个人简介</a></li>
                    <li><a href="#">工作成果</a></li>
                    <li><a href="#">联系我们</a></li>
                </ul>
            </nav>
        </header>

        <!-- 主要内容区域 -->
        <main>
               </main>
        <!-- 底部 -->
 <footer>
            <p>浙江省杭州市西湖区... | 联系电话：... | 邮箱：...</p>
        </footer>
    </div>
    <script>
        // 可以在这里添加JavaScript代码
    </script>
</body>
</html>


    <!-- 页头 -->
    <div class="header">中国金隆之窗</div>

    <!-- 滚动新闻 -->
    <div class="news-ticker">
        <marquee id="news-marquee">加载中...</marquee>
    </div>

    <!-- 滚动天气 -->
    <div class="weather-ticker">
        <marquee id="weather-marquee">天气数据加载中...</marquee>
    </div>

    <!-- 主体内容 -->
    <div class="container">
        <div class="row">
            <!-- 左侧6个模块 -->
            <div class="col-md-6">
                <div class="card mb-3">
                    <div class="card-header">今日头条</div>
                    <div class="card-body">这里是热点新闻内容...</div>
                </div>
                <div class="card mb-3">
                    <div class="card-header">财经分析</div>
                    <div class="card-body">最新的财经动态...</div>
                </div>
                <div class="card mb-3">
                    <div class="card-header">科技创新</div>
                    <div class="card-body">人工智能、5G、芯片最新进展...</div>
                </div>
                <div class="card mb-3">
                    <div class="card-header">生活服务</div>
                    <div class="card-body">健康、教育、房产、交通...</div>
                </div>
                <div class="card mb-3">
                    <div class="card-header">文化艺术</div>
                    <div class="card-body">书画、历史、非遗文化...</div>
                </div>
                <div class="card mb-3">
                    <div class="card-header">体育新闻</div>
                    <div class="card-body">世界杯、奥运会、中超、NBA...</div>
                </div>
            </div>
            
            <!-- 右侧6个模块 -->
            <div class="col-md-6">
                <div class="card mb-3">
                    <div class="card-header">国际观察</div>
                    <div class="card-body">全球热点事件...</div>
                </div>
                <div class="card mb-3">
                    <div class="card-header">社会民生</div>
                    <div class="card-body">社会热点、政策分析...</div>
                </div>
                <div class="card mb-3">
                    <div class="card-header">娱乐八卦</div>
                    <div class="card-body">明星动态、电影综艺...</div>
                </div>
                <div class="card mb-3">
                    <div class="card-header">教育资讯</div>
                    <div class="card-body">高考、考研、留学动态...</div>
                </div>
                <div class="card mb-3">
                    <div class="card-header">本地新闻</div>
                    <div class="card-body">杭州、西湖区最新动态...</div>
                </div>
                <div class="card mb-3">
                    <div class="card-header">旅游推荐</div>
                    <div class="card-body">国内外旅游攻略...</div>
                </div>
            </div>
        </div>
    </div>

    <!-- 底部 -->
    <div class="footer">
        地址：浙江省杭州市西湖区 | 版权所有 © 2025 中国金隆之窗
    </div>

    <script>
        // 模拟百度新闻数据
        let newsData = [
            "中国GDP增长超预期",
            "AI技术突破，GPT-5发布",
            "房价走势分析：哪些城市涨幅最大？",
            "新能源车销量破纪录",
            "2025年高考政策调整",
            "杭州亚运会圆满落幕",
            "全球气候变暖加剧，专家呼吁行动",
            "比特币价格突破6万美元",
            "ChatGPT新版本发布",
            "中国航天新突破，月球基地计划启动"
        ];
        let newsHtml = newsData.map(news => `<span>${news}</span>`).join(" | ");
        $("#news-marquee").html(newsHtml);

        // 模拟天气数据
        let citiesWeather = [
            "北京：晴 8℃",
            "上海：多云 12℃",
            "广州：小雨 18℃",
            "深圳：晴 20℃",
            "杭州：阴 10℃",
            "成都：小雨 11℃",
            "西安：晴 9℃",
            "重庆：多云 13℃",
            "武汉：小雨 10℃",
            "天津：晴 7℃"
        ];
        let weatherHtml = citiesWeather.map(weather => `<span>${weather}</span>`).join(" | ");
        $("#weather-marquee").html(weatherHtml);
    </script>

</body>
</html>
