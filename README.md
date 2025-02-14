<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>中国金隆之窗</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: "Microsoft YaHei", sans-serif;
        }

        body {
            background-color: #f5f5f5;
        }

        .header {
            background-color: #c8161d;
            padding: 15px 0;
            border-bottom: 3px solid #a01318;
        }

        .logo-container {
            width: 1200px;
            margin: 0 auto;
            display: flex;
            align-items: center;
        }

        .logo {
            width: 60px;
            height: 60px;
            background: url('data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADAAAAAwCAYAAABXAvmHAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAAOxAAADsQBlSsOGwAAABl0RVh0U29mdHdhcmUAd3d3Lmlua3NjYXBlLm9yZ5vuPBoAAAJFSURBVGiB7Zk/SAJRFMffUxEKoqGhhqAhaAqCoCGIIAhqCIIgCIIgCIKgoaEhaAiCIAiCIAiChqAhgiAIgiAIgiAIGoKGIPD1HlwPj6v3Tu9eHvh+4MD73Xf3fO/97h1BEARBEARBEARBEARBEARBEARBEARBEARBEARBEARBEARBEARBEARBEH4BxhgxxmKMsWfG2F0Q5w4qgDGWY4y1GGNvjLE3xtgDYyzr97y+BRhjccbYHWNsQERJIkp8Hm8ZY3G/5vYtgIg2iKhPRK/Oc8bYgIjaRLTq19y+BRDRHhG9u5x7I6J9v+b2LYCI1ojo3uXcAxGt+zW3bwFEtE1Ezy7nnoho26+5fQsgoiQR3biceySipF9z+xZARDtE9OJy7p6Idvyae6ECGGMxxtg1Y6zDGFv9PL5gjHUZY1eMsZifc/sWQERrRLRPRIfE6ZCI1v2e17cAIlpmjB0R0RlxOiKiFb/n9S2AiJYYY3kiKnI6JqIlv+f1LYCIYkS0S0QFTnEiivk9t28BjLElIsqRgTKMsSW/5vYtgDG2QkRZ4pQlohW/5vYtgDG2SkQZ4pQhojW/5vYtgDG2TkRp4pQmoqRfc/sWwBjbIKIUcUoR0aZfc/sWwBjbIqJd4rRLRNt+ze1bAGNsj4h2iNMuEe35NbdvAYyxNBHtEKdtIsr4NbdvAYyxLBHtE6cDIjrwK8DzD4kxFmeMXRJRhTG2/nl8QURVIrpgjMV9+QIEQRAEQRAEQRAEQRAEQRAEQRAEQRAEQRAEQRAEQRAEQRAEQRAEQRAEQRAE4T/xDg5+IFvwiQM+AAAAAElFTkSuQmCC') no-repeat;
            background-size: contain;
        }

        .title {
            color: white;
            font-size: 28px;
            margin-left: 15px;
        }

        .nav {
            background-color: #333;
            padding: 10px 0;
        }

        .nav-container {
            width: 1200px;
            margin: 0 auto;
        }

        .nav-item {
            color: white;
            text-decoration: none;
            margin-right: 30px;
            font-size: 16px;
        }

        .main-content {
            width: 1200px;
            margin: 20px auto;
            background-color: white;
            padding: 20px;
        }

        .section-title {
            color: #c8161d;
            border-left: 4px solid #c8161d;
            padding-left: 10px;
            margin: 20px 0;
        }

        .info-box {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 20px;
        }

        .info-item {
            border: 1px solid #eee;
            padding: 15px;
            transition: all 0.3s;
        }

        .info-item:hover {
            box-shadow: 0 2px 12px rgba(0,0,0,0.1);
        }

        .footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 20px 0;
            margin-top: 30px;
        }
    </style>
</head>
<body>
    <header class="header">
        <div class="logo-container">
            <div class="logo"></div>
            <h1 class="title">中国金隆之窗</h1>
        </div>
    </header>

    <nav class="nav">
        <div class="nav-container">
            <a href="#" class="nav-item">首页</a>
            <a href="#" class="nav-item">个人简介</a>
            <a href="#" class="nav-item">项目经验</a>
            <a href="#" class="nav-item">联系方式</a>
        </div>
    </nav>

    <main class="main-content">
        <h2 class="section-title">个人基本信息</h2>
        <div class="info-box">
            <div class="info-item">
                <h3>教育背景</h3>
                <p>XX大学 计算机科学硕士</p>
                <p>2018-2021</p>
            </div>
            <div class="info-item">
                <h3>专业技能</h3>
                <p>Web开发</p>
                <p>数据分析</p>
                <p>项目管理</p>
            </div>
            <div class="info-item">
                <h3>工作经历</h3>
                <p>XX科技 高级工程师</p>
                <p>2021-至今</p>
            </div>
        </div>

        <h2 class="section-title">最新项目</h2>
        <div class="info-box">
            <div class="info-item">
                <h3>智能管理系统</h3>
                <p>项目周期：2023.01-2023.12</p>
                <p>担任角色：项目经理</p>
            </div>
            <div class="info-item">
                <h3>数据分析平台</h3>
                <p>项目周期：2022.06-2022.12</p>
                <p>担任角色：技术负责人</p>
            </div>
        </div>
    </main>

    <footer class="footer">
        <p>版权所有 © 2023 中国金隆之窗 京ICP备12345678号</p>
        <p>联系方式：service@jinlongwindow.cn</p>
    </footer>
</body>
</html>
