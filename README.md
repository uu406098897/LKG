<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>中国金隆之窗</title>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css">
    <script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
    <style>
        /* 页头样式 */
        .header {
            background: linear-gradient(to right, #FF8000, #FFA500);
            color: white;
            padding: 20px;
            text-align: center;
            font-size: 32px;
            font-weight: bold;
        }
        /* 滚动新闻样式 */
        .news-ticker {
            background: #f5f5f5;
            padding: 10px;
            overflow: hidden;
            height: 40px;
            line-height: 40px;
            white-space: nowrap;
            border-bottom: 2px solid #ffa500;
        }
        .news-ticker span {
            display: inline-block;
            padding-right: 50px;
        }
        /* 滚动天气 */
        .weather-ticker {
            overflow: hidden;
            height: 50px;
            white-space: nowrap;
            padding: 10px;
            background: #ececec;
            font-size: 16px;
            border-bottom: 2px solid #ffa500;
        }
        /* 主体内容 */
        .container {
            margin-top: 20px;
            max-width: 1400px;
        }
        .card {
            box-shadow: 2px 2px 10px rgba(0, 0, 0, 0.1);
        }
        /* 底部样式 */
        .footer {
            background: #333;
            color: white;
            text-align: center;
            padding: 15px;
            margin-top: 20px;
        }
    </style>
</head>
<body>

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
                    <div class="card-body">最新国内外热点新闻...</div>
                </div>
                <div class="card mb-3">
                    <div class="card-header">财经分析</div>
                    <div class="card-body">股市、房产、经济动态...</div>
                </div>
                <div class="card mb-3">
                    <div class="card-header">科技创新</div>
                    <div class="card-body">人工智能、5G、芯片技术...</div>
                </div>
                <div class="card mb-3">
                    <div class="card-header">生活服务</div>
                    <div class="card-body">健康、教育、出行、房产...</div>
                </div>
                <div class="card mb-3">
                    <div class="card-header">文化艺术</div>
                    <div class="card-body">书画、历史、传统文化...</div>
                </div>
                <div class="card mb-3">
                    <div class="card-header">体育新闻</div>
                    <div class="card-body">世界杯、奥运会、NBA...</div>
                </div>
            </div>
            
            <!-- 右侧6个模块 -->
            <div class="col-md-6">
                <div class="card mb-3">
                    <div class="card-header">国际观察</div>
                    <div class="card-body">全球热点事件分析...</div>
                </div>
                <div class="card mb-3">
                    <div class="card-header">社会民生</div>
                    <div class="card-body">社会热点、政策解读...</div>
                </div>
                <div class="card mb-3">
                    <div class="card-header">娱乐八卦</div>
                    <div class="card-body">明星动态、影视综艺...</div>
                </div>
                <div class="card mb-3">
                    <div class="card-header">教育资讯</div>
                    <div class="card-body">高考、考研、留学政策...</div>
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
