<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>中国金隆 - 个人信息港</title>
    <style>
        body {
            margin: 0;
            font-family: Arial, sans-serif;
            line-height: 1.6;
        }
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        header {
            background: #333;
            color: white;
            padding: 20px 0;
            text-align: center;
        }
        nav ul {
            list-style: none;
            padding: 0;
            margin: 0;
            display: flex;
            justify-content: center;
        }
        nav ul li {
            margin: 0 15px;
        }
        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: bold;
        }
        .content-block {
            margin: 40px 0;
        }
        .news-scroll {
            height: 80px;
            overflow: hidden;
            position: relative;
            border: 1px solid #ddd;
            padding: 10px;
            margin-top: 30px;
        }
        .news-scroll ul {
            position: absolute;
            animation: scroll 15s linear infinite;
            padding: 0;
            margin: 0;
            list-style: none;
        }
        .news-scroll li {
            height: 30px;
            line-height: 30px;
            margin: 0 0 10px 0;
        }
        @keyframes scroll {
            0% { transform: translateY(0); }
            100% { transform: translateY(-100%); }
        }
        footer {
            background: #f8f8f8;
            padding: 20px 0;
            text-align: center;
            margin-top: 40px;
            color: #666;
        }
        .featured-item {
            border: 1px solid #ddd;
            padding: 20px;
            margin-bottom: 20px;
            border-radius: 8px;
        }
        .featured-item img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 8px;
            margin-bottom: 15px;
        }
        .article-block {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1>中国金隆 - 个人信息港</h1>
            <nav>
                <ul>
                    <li><a href="#profile">个人简介</a></li>
                    <li><a href="#worklife">工作生活</a></li>
                    <li><a href="#honor">个人荣誉</a></li>
                    <li><a href="#dynamic">工作动态</a></li>
                    <li><a href="#news">今日要闻</a></li>
                    <li><a href="#knowledge">个人知识</a></li>
                </ul>
            </nav>
        </header>
        
        <main>
            <div class="content-block" id="profile">
                <h2>个人简介</h2>
                <div class="featured-item">
                    <img src="https://picsum.photos/800/400" alt="个人照片">
                    <h3>金隆</h3>
                    <p>出生于[出生日期]，毕业于[毕业院校]。在[工作行业]领域拥有丰富的工作经验。</p>
                </div>
            </div>
            
            <div class="content-block" id="worklife">
                <h2>工作生活</h2>
                <div class="featured-item">
                    <img src="https://picsum.photos/800/400?random=1" alt="工作生活照">
                    <h3>工作日常</h3>
                    <p>在工作中，我专注于[工作领域]，努力提升专业能力，为工作做出贡献。</p>
                </div>
            </div>
            
            <div class="content-block" id="honor">
                <h2>个人荣誉</h2>
                <div class="featured-item">
                    <h3>2025年度行业创新奖</h3>
                    <p>在[项目名称]项目中，凭借出色的创新能力和专业技能，荣获2025年度行业创新奖。</p>
                </div>
            </div>
            
            <div class="content-block" id="dynamic">
                <h2>工作动态</h2>
                <div class="featured-item">
                    <h3>参与[项目名称]项目</h3>
                    <p>目前正参与[项目名称]项目的开发工作，该项目旨在[项目目标]。</p>
                </div>
            </div>
            
            <div class="news-scroll" id="news">
                <h2>今日要闻</h2>
                <div class="scroll-container">
                    <ul>
                        <li><a href="https://example.com/news1">新闻1：行业动态更新</a></li>
                        <li><a href="https://example.com/news2">新闻2：技术进展分享</a></li>
                        <li><a href="https://example.com/news3">新闻3：行业新政策发布</a></li>
                        <li><a href="https://example.com/news4">新闻4：行业新技术应用</a></li>
                        <li><a href="https://example.com/news5">新闻5：行业新趋势解读</a></li>
                    </ul>
                </div>
            </div>
            
            <div class="content-block" id="knowledge">
                <h2>个人知识</h2>
                <div class="article-block">
                    <div class="featured-item">
                        <h3>技术专题文章</h3>
                        <p>文章内容：详细介绍了[技术领域]的前沿知识和实际应用案例。</p>
                    </div>
                    <div class="featured-item">
                        <h3>行业趋势分析</h3>
                        <p>文章内容：深入分析了当前行业的发展趋势和未来发展方向。</p>
                    </div>
                </div>
            </div>
        </main>
        
        <footer>
            <p>&copy; 2024 中国金隆. 版权所有</p>
            <p>联系我们：contact@example.com</p>
        </footer>
    </div>
</body>
</html>
