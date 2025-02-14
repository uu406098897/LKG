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
                    <li><a href="#">关于我们</a></li>
                    <li><a href="#">产品中心</a></li>
                    <li><a href="#">新闻动态</a></li>
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
<main>
            <section class="module">
                <h2>模块 1：公司简介</h2>
                <p>这里是中国金隆之窗的详细介绍...</p>
            </section>
            <section class="module">
                <h2>模块 2：核心业务</h2>
                <p>详细介绍公司的核心业务范畴...</p>
            </section>
            <section class="module">
                <h2>模块 3：产品展示</h2>
                <p>展示公司的主要产品和服务...</p>
            </section>
            <section class="module">
                <h2>模块 4：技术优势</h2>
                <p>阐述公司的技术实力和竞争优势....</p>
            </section>
            <section class="module">
                <h2>模块 5：团队风采</h2>
                <p>介绍公司的核心团队成员和企业文化...</p>
            </section>
            <section class="module">
                <h2>模块 6：合作伙伴</h2>
                <p>列出公司的主要合作伙伴和客户...</p>
            </section>
            <section class="module">
                <h2>模块 7：新闻资讯</h2>
                <p>发布公司的最新新闻和行业动态...</p>
            </section>
            <section class="module">
                <h2>模块 8：招贤纳士</h2>
                <p>发布公司的招聘信息和人才理念...</p>
            </section>
            <section class="module">
                <h2>模块 9：社会责任</h2>
                <p>展示公司在社会公益方面的贡献...</p>
            </section>
            <section class="module">
                <h2>模块 10：联系方式</h2>
                <p>提供公司的详细联系方式和地址...</p>
            </section>
            <section class="module">
                <h2>模块 11：在线留言</h2>
                <p>设置一个在线留言表单，方便客户咨询...</p>
            </section>
            <section class="module">
                <h2>模块 12：友情链接</h2>
                <p>列出一些相关的友情链接...</p>
            </section>
        </main>
        #baidu-hot-news {
    height: 200px;/*设置高度*/
    overflow: hidden; /* 溢出隐藏 */
}

#baidu-hot-news li{
     height: 20px;
}
<div class="module">
      <h2>主要城市天气</h2>
      <div id="weather-container"></div>
 </div>

<script>
    const city = "beijing,shanghai,guangzhou,shenzhen,hangzhou";
        const apiKey = "在此填写你的API密钥";
        const apiUrl = `https://devapi.qweather.com/v7/weather/now?location=${city}&key=${apiKey}&lang=zh&gzip=n`;
        fetch(apiUrl)
            .then(response => response.json())
            .then(data => {
               console.info(data);
               const wdata = data.now;
               const weatherContainer = document.getElementById('weather-container');
               for(let i in wdata){
                   const cityWeather = document.createElement('div');
                   cityWeather.innerHTML = `<strong>${i}</strong>: ${wdata[i]}`;
                   weatherContainer.appendChild(cityWeather);
               }
            });
</script>
