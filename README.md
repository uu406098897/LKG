<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>中国金隆之窗</title>
    <style>
        /* 基础样式 */
        body {
            margin: 0;
            font-family: '微软雅黑', sans-serif;
            line-height: 1.8;
            background: #f5f5f5;
        }
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
            display: flex;
            gap: 30px;
        }
        header {
            background: linear-gradient(to right, #c0392b, #e67e22);
            color: white;
            padding: 40px 0;
            margin-bottom: 30px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            text-align: center;
        }
        header h1 {
            font-size: 36px;
            margin: 0;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
            letter-spacing: 2px;
        }
        nav {
            background: rgba(0,0,0,0.1);
            padding: 15px 0;
            margin-top: 20px;
        }
        nav ul {
            list-style: none;
            padding: 0;
            margin: 0;
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
        }
        nav ul li {
            margin: 0 15px;
        }
        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: bold;
            padding: 8px 15px;
            border-radius: 5px;
            transition: background 0.3s;
        }
        nav ul li a:hover {
            background: rgba(255,255,255,0.2);
        }
        .content-block {
            background: white;
            margin: 25px 0;
            padding: 30px;
            border-radius: 12px;
            box-shadow: 0 2px 15px rgba(0,0,0,0.08);
        }
        .news-scroll {
            height: 50px;
            overflow: hidden;
            position: relative;
            background: #fff;
            border-radius: 8px;
            margin: 20px 0;
        }
        .news-scroll ul {
            position: absolute;
            white-space: nowrap;
            padding: 15px 0;
            margin: 0;
            animation: scroll 25s linear infinite;
        }
        .news-scroll li {
            display: inline-block;
            margin-right: 50px;
            font-size: 16px;
        }
        .news-scroll a {
            color: #e74c3c;
            text-decoration: none;
            transition: color 0.3s;
        }
        .news-scroll a:hover {
            color: #c0392b;
            text-decoration: underline;
        }
        @keyframes scroll {
            0% { transform: translateX(100%); }
            100% { transform: translateX(-100%); }
        }
        .featured-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 25px;
            margin-top: 20px;
        }
        .featured-item {
            background: #fff;
            border-radius: 10px;
            padding: 20px;
            transition: transform 0.3s;
            border: 1px solid #eee;
        }
        .featured-item:hover {
            transform: translateY(-5px);
        }
        .featured-item img {
            width: 100%;
            height: 180px;
            object-fit: cover;
            border-radius: 8px;
            margin-bottom: 15px;
        }
        footer {
            background: #333;
            color: #fff;
            padding: 40px 0;
            margin-top: 50px;
            text-align: center;
        }
        h2 {
            color: #e67e22;
            border-left: 5px solid #c0392b;
            padding-left: 15px;
            margin: 25px 0;
        }
        /* 新增侧边栏样式 */
        .sidebar {
            width: 300px;
            background: #fff;
            border-radius: 12px;
            padding: 20px;
            box-shadow: 0 2px 15px rgba(0,0,0,0.08);
        }
        .weather-module {
            margin-top: 20px;
            padding: 15px;
            background: #f1f1f1;
            border-radius: 8px;
        }
        .weather-module h3 {
            margin: 0 0 10px;
        }
        .weather-module p {
            margin: 5px 0;
        }
    </style>
</head>
<body>
    <header>
        <h1>中国金隆之窗</h1>
        <nav>
            <ul>
                <li><a href="#profile">个人简介</a></li>
                <li><a href="#skills">核心能力</a></li>
                <li><a href="#projects">项目成果</a></li>
                <li><a href="#gallery">作品展示</a></li>
                <li><a href="#resources">资源推荐</a></li>
            </ul>
        </nav>
    </header>
    <div class="container">
        <!-- 左侧栏 -->
        <aside class="sidebar">
            <div class="news-scroll">
                <ul>
                    <li><a href="https://example.com/pm" target="_blank">🔥 2025年项目管理趋势报告发布</a></li>
                    <li><a href="https://example.com/agile" target="_blank">🌟 敏捷开发与项目管理结合新方法</a></li>
                    <li><a href="https://example.com/remote" target="_blank">🚀 远程团队管理工具推荐</a></li>
                    <li><a href="https://example.com/risk" target="_blank">⚠️ 项目风险管理最佳实践</a></li>
                </ul>
            </div>
            <div class="weather-module">
                <h3>今日天气</h3>
                <p>北京：晴，15°C - 25°C</p>
                <p>空气质量：优</p>
                <p>湿度：45%</p>
            </div>
        </aside>
        <!-- 主内容区 -->
        <main style="flex-grow: 1;">
            <!-- 模块1：个人简介 -->
            <div class="content-block" id="profile">
                <h2>个人简介</h2>
                <div class="featured-grid">
                    <div class="featured-item">
                        <img src="https://picsum.photos/id/1018/800/400" alt="专业形象照">
                        <h3>金隆 | 项目管理专家</h3>
                        <p>🔹 大连工业大学艺术设计硕士<br>
                           🔹 国家级项目管理认证（PMP）<br>
                           🔹 艺术设计与项目管理领域专家<br>
                           🔹 10年项目管理与团队协作经验</p>
                    </div>
                </div>
            </div>

            <!-- 模块2：核心能力 -->
            <div class="content-block" id="skills">
                <h2>核心能力</h2>
                <div class="featured-grid">
                    <div class="featured-item">
                        <h3>📊 项目规划</h3>
                        <p>• 制定清晰的项目目标与里程碑<br>
                           • 使用甘特图进行任务分解<br>
                           • 确保资源分配合理高效</p>
                    </div>
                    <div class="featured-item">
                        <h3>👥 团队协作</h3>
                        <p>• 建立高效的跨职能团队<br>
                           • 使用敏捷开发提升团队效率<br>
                           • 定期组织项目复盘与优化</p>
                    </div>
                </div>
            </div>

            <!-- 模块3：项目成果 -->
            <div class="content-block" id="projects">
                <h2>代表项目</h2>
                <div class="featured-grid">
                    <div class="featured-item">
                        <img src="https://picsum.photos/id/1015/800/400" alt="展览设计项目">
                        <h3>大型展览设计项目</h3>
                        <p>• 项目周期：2022-2023<br>
                           • 核心技术：项目管理+设计创新<br>
                           • 成效：客户满意度达95%</p>
                    </div>
                    <div class="featured-item">
                        <img src="https://picsum.photos/id/1025/800/400" alt="品牌重塑项目">
                        <h3>品牌重塑项目</h3>
                        <p>• 客户：某知名快消品牌<br>
                           • 目标：品牌形象升级<br>
                           • 成果：销售额增长20%</p>
                    </div>
                </div>
            </div>

            <!-- 模块4：作品展示 -->
            <div class="content-block" id="gallery">
                <h2>作品展示</h2>
                <div class="featured-grid">
                    <div class="featured-item">
                        <img src="https://picsum.photos/id/1035/800/400" alt="艺术作品1">
                        <h3>艺术作品1</h3>
                        <p>描述：现代风格的艺术设计作品。</p>
                    </div>
                    <div class="featured-item">
                        <img src="https://picsum.photos/id/1045/800/400" alt="艺术作品2">
                        <h3>艺术作品2</h3>
                        <p>描述：简约风格的设计案例。</p>
                    </div>
                </div>
            </div>

            <!-- 模块5：资源推荐 -->
            <div class="content-block" id="resources">
                <h2>资源推荐</h2>
                <div class="featured-grid">
                    <div class="featured-item">
                        <h3>📚 书籍推荐</h3>
                        <p>《敏捷项目管理》 - 作者：XXX</p>
                    </div>
                    <div class="featured-item">
                        <h3>🔗 在线课程</h3>
                        <p>《项目管理基础》 - 平台：Coursera</p>
                    </div>
                </div>
            </div>

            <!-- 其他模块 -->
            <div class="content-block">
                <h2>其他模块</h2>
                <div class="featured-grid">
                    <div class="featured-item">
                        <img src="https://picsum.photos/id/1055/800/400" alt="自然风光">
                        <h3>自然风光</h3>
                        <p>描述：美丽的自然景观摄影作品。</p>
                    </div>
                    <div class="featured-item">
                        <img src="https://picsum.photos/id/1065/800/400" alt="城市建筑">
                        <h3>城市建筑</h3>
                        <p>描述：现代城市的建筑设计。</p>
                    </div>
                </div>
            </div>
        </main>
    </div>
    <footer>
        <p>© 2025 中国金隆创新研究院 版权所有</p>
        <p>学术合作：research@jinlong.cn | 媒体联络：press@jinlong.cn</p>
        <p>地址：北京市海淀区人工智能产业园A座</p>
    </footer>
</body>
</html>
