<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>中国金隆之窗</title>
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
            box-sizing: border-box;
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
            margin: 20px 0;
        }
        .news-scroll {
            height: 40px;
            overflow: hidden;
            white-space: nowrap;
            border: 1px solid #ddd;
            padding: 10px;
            margin: 10px 0;
        }
        .news-scroll ul {
            display: inline-block;
            animation: scroll 30s linear infinite;
            padding: 0;
            margin: 0;
            list-style: none;
        }
        .news-scroll li {
            display: inline-block;
            margin-right: 20px;
        }
        @keyframes scroll {
            0% { transform: translateX(100%); }
            100% { transform: translateX(-100%); }
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
            padding: 10px;
            margin-bottom: 10px;
            border-radius: 8px;
            width: calc(33.33% - 10px);
            float: left;
            margin-right: 10px;
        }
        .featured-item:nth-child(3n) {
            margin-right: 0;
        }
        .featured-item img {
            width: 100%;
            height: 150px;
            object-fit: cover;
            border-radius: 8px;
            margin-bottom: 5px;
        }
        .article-block {
            overflow: hidden;
            clear: both;
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
                <div class="article-block">
                    <div class="featured-item">
                        <img src="https://picsum.photos/800/400?random=1" alt="工作生活照">
                        <h3>工作日常</h3>
                        <p>在工作中，我专注于[工作领域]，努力提升专业能力，为工作做出贡献。</p>
                    </div>
                    <div class="featured-item">
                        <img src="https://picsum.photos/800/400?random=2" alt="工作生活照">
                        <h3>生活点滴</h3>
                        <p>在生活中，我喜欢阅读和旅行，这些经历使我不断成长和进步。</p>
                    </div>
                    <div class="featured-item">
                        <img src="https://picsum.photos/800/400?random=3" alt="工作生活照">
                        <h3>团队合作</h3>
                        <p>我相信团队的力量，与同事携手共同完成项目，创造更多价值。</p>
                    </div>
                </div>
            </div>
            
            <div class="content-block" id="honor">
                <h2>个人荣誉</h2>
                <div class="article-block">
                    <div class="featured-item">
                        <h3>2025年度行业创新奖</h3>
                        <p>在[项目名称]项目中，凭借出色的创新能力和专业技能，荣获2025年度行业创新奖。</p>
                    </div>
                    <div class="featured-item">
                        <h3>2024年度优秀员工</h3>
                        <p>在公司评选中，被评为2024年度优秀员工，为公司的发展做出突出贡献。</p>
                    </div>
                    <div class="featured-item">
                        <h3>2023年度优秀论文奖</h3>
                        <p>撰写的论文《[论文标题]》在行业学术会议中荣获2023年度优秀论文奖。</p>
                    </div>
                </div>
            </div>
            
            <div class="content-block" id="dynamic">
                <h2>工作动态</h2>
                <div class="article-block">
                    <div class="featured-item">
                        <h3>参与[项目名称]项目</h3>
                        <p>目前正参与[项目名称]项目的开发工作，该项目旨在[项目目标]。</p>
                    </div>
                    <div class="featured-item">
                        <h3>出席行业研讨会</h3>
                        <p>近期，受邀出席了[研讨会名称]行业研讨会，在会上分享了专业见解和经验。</p>
                    </div>
                    <div class="featured-item">
                        <h3>团队培训计划</h3>
                        <p>制定了团队培训计划，旨在提升团队成员的工作技能和专业素养。</p>
                    </div>
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
                    <div class="featured-item">
                        <h3>案例研究分享</h3>
                        <p>文章内容：分享了[案例名称]案例研究，从实践中总结经验和教训。</p>
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
