<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>次元小屋 - 二次元爱好者聚集地</title>
    <!-- 简化样式，仅保留核心布局 -->
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: "Microsoft Yahei", sans-serif;
        }
        
        body {
            background-color: #f8f9fa;
            color: #333;
        }
        
        /* 导航栏 */
        header {
            background-color: #fff;
            box-shadow: 0 2px 8px rgba(0,0,0,0.1);
            padding: 15px 0;
            position: sticky;
            top: 0;
            z-index: 999;
        }
        
        .nav-container {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 0 20px;
        }
        
        .logo {
            color: #e53e3e;
            font-size: 24px;
            font-weight: bold;
            text-decoration: none;
        }
        
        .nav-links a {
            margin-left: 30px;
            text-decoration: none;
            color: #333;
            font-size: 16px;
        }
        
        .nav-links a:hover {
            color: #e53e3e;
        }
        
        /* 轮播区 */
        .banner {
            height: 400px;
            background: url('https://picsum.photos/id/237/1920/400') no-repeat center;
            background-size: cover;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #fff;
            text-align: center;
        }
        
        .banner h1 {
            font-size: 40px;
            text-shadow: 0 2px 4px rgba(0,0,0,0.5);
            margin-bottom: 20px;
        }
        
        .banner p {
            font-size: 18px;
            text-shadow: 0 2px 4px rgba(0,0,0,0.5);
            max-width: 600px;
        }
        
        /* 内容区 */
        .container {
            max-width: 1200px;
            margin: 40px auto;
            padding: 0 20px;
        }
        
        .section-title {
            font-size: 28px;
            margin-bottom: 30px;
            color: #333;
            border-left: 4px solid #e53e3e;
            padding-left: 15px;
        }
        
        /* 作品展示 */
        .works-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 20px;
        }
        
        .work-card {
            background: #fff;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 2px 8px rgba(0,0,0,0.1);
            transition: transform 0.3s;
        }
        
        .work-card:hover {
            transform: translateY(-5px);
        }
        
        .work-img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }
        
        .work-info {
            padding: 15px;
        }
        
        .work-title {
            font-size: 18px;
            font-weight: bold;
            margin-bottom: 8px;
        }
        
        .work-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
            margin-top: 10px;
        }
        
        .tag {
            font-size: 12px;
            padding: 3px 8px;
            background: #f0f0f0;
            border-radius: 4px;
            color: #666;
        }
        
        /* 页脚 */
        footer {
            background-color: #333;
            color: #fff;
            padding: 40px 0;
            margin-top: 60px;
        }
        
        .footer-container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
            text-align: center;
        }
        
        .footer-container p {
            margin-top: 15px;
            font-size: 14px;
            color: #ccc;
        }
        
        /* 移动端适配 */
        @media (max-width: 768px) {
            .nav-links {
                display: none;
            }
            .banner {
                height: 250px;
            }
            .banner h1 {
                font-size: 28px;
            }
            .banner p {
                font-size: 16px;
            }
            .section-title {
                font-size: 24px;
            }
        }
    </style>
</head>
<body>
    <!-- 导航栏 -->
    <header>
        <div class="nav-container">
            <a href="#" class="logo">次元小屋</a>
            <div class="nav-links">
                <a href="#home">首页</a>
                <a href="#works">热门作品</a>
                <a href="#about">关于我们</a>
            </div>
        </div>
    </header>

    <!-- 轮播/横幅 -->
    <section id="home" class="banner">
        <div>
            <h1>欢迎来到次元小屋</h1>
            <p>精选优质二次元作品，和同好一起分享热爱</p>
        </div>
    </section>

    <!-- 主要内容 -->
    <div class="container">
        <!-- 热门作品区 -->
        <section id="works">
            <h2 class="section-title">热门作品</h2>
            <div class="works-grid">
                <!-- 作品卡片1 -->
                <div class="work-card">
                    <img src="https://picsum.photos/id/1/500/300" alt="原神" class="work-img">
                    <div class="work-info">
                        <h3 class="work-title">原神</h3>
                        <p>开放世界冒险游戏，探索提瓦特大陆</p>
                        <div class="work-tags">
                            <span class="tag">冒险</span>
                            <span class="tag">奇幻</span>
                            <span class="tag">角色扮演</span>
                        </div>
                    </div>
                </div>
                
                <!-- 作品卡片2 -->
                <div class="work-card">
                    <img src="https://picsum.photos/id/2/500/300" alt="鬼灭之刃" class="work-img">
                    <div class="work-info">
                        <h3 class="work-title">鬼灭之刃</h3>
                        <p>热血战斗番，斩杀恶鬼守护家人</p>
                        <div class="work-tags">
                            <span class="tag">战斗</span>
                            <span class="tag">热血</span>
                            <span class="tag">奇幻</span>
                        </div>
                    </div>
                </div>
                
                <!-- 作品卡片3 -->
                <div class="work-card">
                    <img src="https://picsum.photos/id/3/500/300" alt="星穹铁道" class="work-img">
                    <div class="work-info">
                        <h3 class="work-title">崩坏：星穹铁道</h3>
                        <p>银河冒险RPG，探索宇宙的奥秘</p>
                        <div class="work-tags">
                            <span class="tag">科幻</span>
                            <span class="tag">冒险</span>
                            <span class="tag">回合制</span>
                        </div>
                    </div>
                </div>
                
                <!-- 作品卡片4 -->
                <div class="work-card">
                    <img src="https://picsum.photos/id/4/500/300" alt="咒术回战" class="work-img">
                    <div class="work-info">
                        <h3 class="work-title">咒术回战</h3>
                        <p>少年们与诅咒的战斗物语</p>
                        <div class="work-tags">
                            <span class="tag">战斗</span>
                            <span class="tag">悬疑</span>
                            <span class="tag">校园</span>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- 关于我们 -->
        <section id="about" style="margin-top: 60px;">
            <h2 class="section-title">关于我们</h2>
            <p style="line-height: 1.8; font-size: 16px;">
                次元小屋是一个专注于二次元内容分享的平台，致力于为广大二次元爱好者提供优质的作品推荐、
                角色介绍和同好交流空间。我们精选各类热门动漫、游戏、漫画作品，
                希望能让每一位爱好者都能在这里找到属于自己的快乐。
            </p>
        </section>
    </div>

    <!-- 页脚 -->
    <footer>
        <div class="footer-container">
            <h3>次元小屋</h3>
            <p>© 2025 次元小屋 版权所有</p>
        </div>
    </footer>
</body>
</html>
