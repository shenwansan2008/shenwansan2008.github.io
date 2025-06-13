
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>王伟（云洲） - 金融科技运营专家</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary: #0a192f;      /* 深蓝色 - 专业稳重 */
            --secondary: #d4af37;    /* 金色 - 金融科技专业感 */
            --accent: #64b5f6;       /* 浅蓝色 - 科技感 */
            --light: #f8f9fa;        /* 浅灰背景 */
            --dark: #212529;         /* 深灰文字 */
            --transition: all 0.3s ease;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', 'Microsoft YaHei', sans-serif;
        }
        
        body {
            background-color: #f0f2f5;
            color: var(--dark);
            line-height: 1.6;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* 头部导航 */
        header {
            background-color: var(--primary);
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }
        
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 0;
        }
        
        .logo {
            color: white;
            font-size: 1.8rem;
            font-weight: 700;
            text-decoration: none;
        }
        
        .logo span {
            color: var(--secondary);
        }
        
        .nav-links {
            display: flex;
            list-style: none;
        }
        
        .nav-links li {
            margin-left: 30px;
        }
        
        .nav-links a {
            color: white;
            text-decoration: none;
            font-weight: 500;
            font-size: 1.1rem;
            transition: var(--transition);
            position: relative;
            padding-bottom: 5px;
        }
        
        .nav-links a:hover {
            color: var(--secondary);
        }
        
        .nav-links a::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 0;
            height: 2px;
            background-color: var(--secondary);
            transition: var(--transition);
        }
        
        .nav-links a:hover::after {
            width: 100%;
        }
        
        .menu-toggle {
            display: none;
            color: white;
            font-size: 1.5rem;
            cursor: pointer;
        }
        
        /* 个人简介部分 */
        .hero {
            background: linear-gradient(135deg, var(--primary) 0%, #162b4d 100%);
            color: white;
            padding: 180px 0 100px;
            text-align: center;
            position: relative;
            overflow: hidden;
        }
        
        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100" preserveAspectRatio="none"><polygon fill="rgba(10,25,47,0.8)" points="0,100 100,0 100,100"/></svg>');
            background-size: 100% 100%;
            opacity: 0.2;
        }
        
        .hero-content {
            position: relative;
            z-index: 2;
            max-width: 800px;
            margin: 0 auto;
        }
        
        .profile-img {
            width: 180px;
            height: 180px;
            border-radius: 50%;
            border: 5px solid rgba(255,255,255,0.2);
            margin: 0 auto 25px;
            background: linear-gradient(45deg, var(--secondary), var(--accent));
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 5rem;
            color: white;
        }
        
        .hero h1 {
            font-size: 3.5rem;
            margin-bottom: 15px;
            letter-spacing: 1px;
        }
        
        .hero h2 {
            font-size: 1.8rem;
            color: var(--secondary);
            font-weight: 400;
            margin-bottom: 25px;
        }
        
        .hero p {
            font-size: 1.2rem;
            max-width: 700px;
            margin: 0 auto 30px;
            opacity: 0.9;
        }
        
        .contact-badge {
            display: inline-flex;
            align-items: center;
            background: rgba(255,255,255,0.1);
            padding: 12px 25px;
            border-radius: 50px;
            margin: 5px 10px;
            transition: var(--transition);
        }
        
        .contact-badge:hover {
            background: rgba(255,255,255,0.2);
            transform: translateY(-3px);
        }
        
        .contact-badge i {
            margin-right: 10px;
            color: var(--secondary);
        }
        
        /* 技能特长部分 */
        .skills {
            padding: 100px 0;
            background-color: var(--light);
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 60px;
            position: relative;
        }
        
        .section-title h2 {
            font-size: 2.5rem;
            color: var(--primary);
            display: inline-block;
            margin-bottom: 15px;
        }
        
        .section-title h2::after {
            content: '';
            display: block;
            width: 70px;
            height: 4px;
            background: var(--secondary);
            margin: 15px auto;
            border-radius: 2px;
        }
        
        .section-title p {
            color: #666;
            max-width: 700px;
            margin: 0 auto;
            font-size: 1.1rem;
        }
        
        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin-top: 50px;
        }
        
        .skill-category {
            background: white;
            border-radius: 10px;
            padding: 30px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            transition: var(--transition);
        }
        
        .skill-category:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0,0,0,0.1);
        }
        
        .skill-category h3 {
            color: var(--primary);
            font-size: 1.5rem;
            margin-bottom: 20px;
            display: flex;
            align-items: center;
        }
        
        .skill-category h3 i {
            margin-right: 10px;
            color: var(--secondary);
        }
        
        .skill-item {
            margin-bottom: 20px;
        }
        
        .skill-header {
            display: flex;
            justify-content: space-between;
            margin-bottom: 8px;
        }
        
        .skill-bar {
            height: 8px;
            background-color: #e9ecef;
            border-radius: 4px;
            overflow: hidden;
        }
        
        .skill-progress {
            height: 100%;
            background: linear-gradient(90deg, var(--secondary), var(--accent));
            border-radius: 4px;
        }
        
        /* 项目经历部分 */
        .projects {
            padding: 100px 0;
            background-color: white;
        }
        
        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 40px;
        }
        
        .project-card {
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.08);
            transition: var(--transition);
            background: white;
        }
        
        .project-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0,0,0,0.12);
        }
        
        .project-img {
            height: 200px;
            background: linear-gradient(45deg, var(--primary), #1a3a6b);
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 3rem;
        }
        
        .project-content {
            padding: 25px;
        }
        
        .project-content h3 {
            color: var(--primary);
            font-size: 1.5rem;
            margin-bottom: 15px;
        }
        
        .project-content p {
            color: #666;
            margin-bottom: 20px;
        }
        
        .project-stats {
            display: flex;
            justify-content: space-between;
            background: rgba(10,25,47,0.03);
            padding: 15px;
            border-radius: 8px;
            margin-top: 20px;
        }
        
        .stat-item {
            text-align: center;
        }
        
        .stat-item .number {
            font-size: 1.8rem;
            font-weight: 700;
            color: var(--secondary);
        }
        
        .stat-item .label {
            font-size: 0.9rem;
            color: #666;
        }
        
        /* 联系方式部分 */
        .contact {
            padding: 100px 0;
            background: linear-gradient(135deg, var(--primary) 0%, #162b4d 100%);
            color: white;
            position: relative;
            overflow: hidden;
        }
        
        .contact::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100" preserveAspectRatio="none"><polygon fill="rgba(10,25,47,0.8)" points="0,0 100,100 0,100"/></svg>');
            background-size: 100% 100%;
            opacity: 0.2;
        }
        
        .contact-content {
            position: relative;
            z-index: 2;
            display: flex;
            flex-wrap: wrap;
            gap: 50px;
        }
        
        .contact-info {
            flex: 1;
            min-width: 300px;
        }
        
        .contact-info h2 {
            font-size: 2.5rem;
            margin-bottom: 25px;
            position: relative;
            display: inline-block;
        }
        
        .contact-info h2::after {
            content: '';
            display: block;
            width: 70px;
            height: 4px;
            background: var(--secondary);
            margin-top: 15px;
            border-radius: 2px;
        }
        
        .contact-info p {
            margin-bottom: 30px;
            font-size: 1.1rem;
            max-width: 500px;
            opacity: 0.9;
        }
        
        .contact-details {
            margin-top: 30px;
        }
        
        .contact-item {
            display: flex;
            align-items: flex-start;
            margin-bottom: 25px;
        }
        
        .contact-item i {
            font-size: 1.5rem;
            color: var(--secondary);
            min-width: 50px;
            padding-top: 5px;
        }
        
        .contact-item-content h4 {
            font-size: 1.2rem;
            margin-bottom: 5px;
        }
        
        .contact-item-content p {
            margin: 0;
            opacity: 0.8;
        }
        
        .social-links {
            display: flex;
            margin-top: 30px;
            gap: 15px;
        }
        
        .social-link {
            display: flex;
            align-items: center;
            justify-content: center;
            width: 50px;
            height: 50px;
            border-radius: 50%;
            background: rgba(255,255,255,0.1);
            color: white;
            font-size: 1.3rem;
            transition: var(--transition);
        }
        
        .social-link:hover {
            background: var(--secondary);
            transform: translateY(-5px);
        }
        
        .qrcode-section {
            flex: 1;
            min-width: 300px;
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        
        .qrcode {
            width: 200px;
            height: 200px;
            background: linear-gradient(45deg, var(--secondary), var(--accent));
            border-radius: 10px;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-bottom: 25px;
            font-size: 1.5rem;
            color: white;
        }
        
        .qrcode-label {
            font-size: 1.1rem;
            text-align: center;
            opacity: 0.9;
        }
        
        /* 页脚 */
        footer {
            background: #0a0f1c;
            color: rgba(255,255,255,0.6);
            padding: 30px 0;
            text-align: center;
            font-size: 0.9rem;
        }
        
        /* 响应式设计 */
        @media (max-width: 992px) {
            .hero h1 {
                font-size: 2.8rem;
            }
            
            .section-title h2 {
                font-size: 2rem;
            }
        }
        
        @media (max-width: 768px) {
            .menu-toggle {
                display: block;
            }
            
            .nav-links {
                position: absolute;
                top: 100%;
                left: 0;
                width: 100%;
                background: var(--primary);
                flex-direction: column;
                align-items: center;
                padding: 20px 0;
                clip-path: polygon(0 0, 100% 0, 100% 0, 0 0);
                transition: var(--transition);
            }
            
            .nav-links.active {
                clip-path: polygon(0 0, 100% 0, 100% 100%, 0 100%);
            }
            
            .nav-links li {
                margin: 15px 0;
            }
            
            .hero {
                padding: 150px 0 80px;
            }
            
            .hero h1 {
                font-size: 2.3rem;
            }
            
            .hero h2 {
                font-size: 1.5rem;
            }
            
            .contact-badge {
                display: block;
                margin: 10px auto;
                max-width: 300px;
            }
        }
        
        @media (max-width: 576px) {
            .profile-img {
                width: 150px;
                height: 150px;
                font-size: 4rem;
            }
            
            .hero h1 {
                font-size: 2rem;
            }
            
            .section-title h2 {
                font-size: 1.8rem;
            }
            
            .project-img {
                height: 180px;
            }
        }
    </style>
</head>
<body>
    <!-- 导航栏 -->
    <header>
        <div class="container">
            <nav>
                <a href="#" class="logo">王<span>伟</span></a>
                <div class="menu-toggle" id="menuToggle">
                    <i class="fas fa-bars"></i>
                </div>
                <ul class="nav-links" id="navLinks">
                    <li><a href="#about">个人简介</a></li>
                    <li><a href="#skills">技能特长</a></li>
                    <li><a href="#projects">项目经历</a></li>
                    <li><a href="#contact">联系方式</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- 个人简介 -->
    <section class="hero" id="about">
        <div class="container">
            <div class="hero-content">
                <div class="profile-img">
                    <i class="fas fa-user"></i>
                </div>
                <h1>王伟</h1>
                <h2>互联网产品运营总监 | 资深互金运营专家</h2>
                <p>互联网金融产品运营总监、前阿里/蚂蚁集团资深产品运营专家、杭州高层次人才。10年+金融科技/O2O电商背景，2家互联网上市公司及一线大厂运营管理经验，拥有体系化的产品运营管理方法论。</p>
                
                <div class="contact-badges">
                    <a href="tel:18557519167" class="contact-badge">
                        <i class="fas fa-phone"></i>185-5751-9167（微信同号）
                    </a>
                    <a href="mailto:shenwansan2008@163.com" class="contact-badge">
                        <i class="fas fa-envelope"></i>shenwansan2008@163.com
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- 技能特长 -->
    <section class="skills" id="skills">
        <div class="container">
            <div class="section-title">
                <h2>技能特长</h2>
                <p>在金融科技领域拥有丰富的产品运营和项目经验，擅长用户增长、产品运营、团队及项目管理</p>
            </div>
            
            <div class="skills-grid">
                <div class="skill-category">
                    <h3><i class="fas fa-users"></i>用户运营能力</h3>
                    <div class="skill-item">
                        <div class="skill-header">
                            <span>用户增长体系搭建</span>
                            <span>95%</span>
                        </div>
                        <div class="skill-bar">
                            <div class="skill-progress" style="width: 95%"></div>
                        </div>
                    </div>
                    <div class="skill-item">
                        <div class="skill-header">
                            <span>用户生命周期管理</span>
                            <span>92%</span>
                        </div>
                        <div class="skill-bar">
                            <div class="skill-progress" style="width: 92%"></div>
                        </div>
                    </div>
                    <div class="skill-item">
                        <div class="skill-header">
                            <span>活动策划与执行</span>
                            <span>90%</span>
                        </div>
                        <div class="skill-bar">
                            <div class="skill-progress" style="width: 90%"></div>
                        </div>
                    </div>
                    <div class="skill-item">
                        <div class="skill-header">
                            <span>精准营销策略</span>
                            <span>88%</span>
                        </div>
                        <div class="skill-bar">
                            <div class="skill-progress" style="width: 88%"></div>
                        </div>
                    </div>
                </div>
                
                <div class="skill-category">
                    <h3><i class="fas fa-chart-line"></i>产品运营能力</h3>
                    <div class="skill-item">
                        <div class="skill-header">
                            <span>产品迭代优化</span>
                            <span>90%</span>
                        </div>
                        <div class="skill-bar">
                            <div class="skill-progress" style="width: 90%"></div>
                        </div>
                    </div>
                    <div class="skill-item">
                        <div class="skill-header">
                            <span>数据分析与BI工具</span>
                            <span>85%</span>
                        </div>
                        <div class="skill-bar">
                            <div class="skill-progress" style="width: 85%"></div>
                        </div>
                    </div>
                    <div class="skill-item">
                        <div class="skill-header">
                            <span>需求策划与用户洞察</span>
                            <span>93%</span>
                        </div>
                        <div class="skill-bar">
                            <div class="skill-progress" style="width: 93%"></div>
                        </div>
                    </div>
                    <div class="skill-item">
                        <div class="skill-header">
                            <span>AB测试与实验设计</span>
                            <span>87%</span>
                        </div>
                        <div class="skill-bar">
                            <div class="skill-progress" style="width: 87%"></div>
                        </div>
                    </div>
                </div>
                
                <div class="skill-category">
                    <h3><i class="fas fa-project-diagram"></i>团队与项目管理</h3>
                    <div class="skill-item">
                        <div class="skill-header">
                            <span>跨部门协作</span>
                            <span>92%</span>
                        </div>
                        <div class="skill-bar">
                            <div class="skill-progress" style="width: 92%"></div>
                        </div>
                    </div>
                    <div class="skill-item">
                        <div class="skill-header">
                            <span>团队建设与管理</span>
                            <span>90%</span>
                        </div>
                        <div class="skill-bar">
                            <div class="skill-progress" style="width: 90%"></div>
                        </div>
                    </div>
                    <div class="skill-item">
                        <div class="skill-header">
                            <span>战略规划与执行</span>
                            <span>94%</span>
                        </div>
                        <div class="skill-bar">
                            <div class="skill-progress" style="width: 94%"></div>
                        </div>
                    </div>
                    <div class="skill-item">
                        <div class="skill-header">
                            <span>KPI设定与达成</span>
                            <span>95%</span>
                        </div>
                        <div class="skill-bar">
                            <div class="skill-progress" style="width: 95%"></div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 项目经历 -->
    <section class="projects" id="projects">
        <div class="container">
            <div class="section-title">
                <h2>代表项目</h2>
                <p>在职业生涯中成功主导并完成了多个具有重要影响力的项目</p>
            </div>
            
            <div class="projects-grid">
                <div class="project-card">
                    <div class="project-img">
                        <i class="fas fa-chart-network"></i>
                    </div>
                    <div class="project-content">
                        <h3>51人品专家（用户增长）</h3>
                        <p>通过用户MGM分享裂变机制设计，从0到1构建用户增长裂变模块。创新性地结合社交裂变与金融产品特性，实现用户自发传播。</p>
                        <div class="project-stats">
                            <div class="stat-item">
                                <div class="number">33%</div>
                                <div class="label">平台新用户占比</div>
                            </div>
                            <div class="stat-item">
                                <div class="number">10K+</div>
                                <div class="label">月均裂变用户</div>
                            </div>
                        </div>
                    </div>
                </div>
                
                <div class="project-card">
                    <div class="project-img">
                        <i class="fas fa-handshake"></i>
                    </div>
                    <div class="project-content">
                        <h3>支付宝&KFC联合会员</h3>
                        <p>通过阿里巴巴-本地生活CRM精准营销运营，实现品牌联合会员体系打通。创新会员权益设计，提升用户转化与品牌忠诚度。</p>
                        <div class="project-stats">
                            <div class="stat-item">
                                <div class="number">50K+</div>
                                <div class="label">单日拉新会员</div>
                            </div>
                            <div class="stat-item">
                                <div class="number">666</div>
                                <div class="label">联名会员卡</div>
                            </div>
                        </div>
                    </div>
                </div>
                
                <div class="project-card">
                    <div class="project-img">
                        <i class="fas fa-coins"></i>
                    </div>
                    <div class="project-content">
                        <h3>网商银行2021丰收节</h3>
                        <p>针对农村金融需求策划节点营销活动，借助支付宝流量精准触达目标客户。创新信贷产品设计，提升三农客户金融服务可及性。</p>
                        <div class="project-stats">
                            <div class="stat-item">
                                <div class="number">25亿+</div>
                                <div class="label">信贷支持金额</div>
                            </div>
                            <div class="stat-item">
                                <div class="number">8万+</div>
                                <div class="label">转化客户数</div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 联系方式 -->
    <section class="contact" id="contact">
        <div class="container">
            <div class="contact-content">
                <div class="contact-info">
                    <h2>联系我</h2>
                    <p>如果您对金融科技产品运营、用户增长策略或团队管理有任何问题或合作意向，欢迎随时与我联系</p>
                    
                    <div class="contact-details">
                        <div class="contact-item">
                            <i class="fas fa-phone"></i>
                            <div class="contact-item-content">
                                <h4>电话/微信</h4>
                                <p>185-5751-9167</p>
                            </div>
                        </div>
                        
                        <div class="contact-item">
                            <i class="fas fa-envelope"></i>
                            <div class="contact-item-content">
                                <h4>电子邮箱</h4>
                                <p>shenwansan2008@163.com</p>
                            </div>
                        </div>
                        
                        <div class="contact-item">
                            <i class="fas fa-map-marker-alt"></i>
                            <div class="contact-item-content">
                                <h4>所在地</h4>
                                <p>杭州 | 西湖区</p>
                            </div>
                        </div>
                        
                        <div class="contact-item">
                            <i class="fab fa-weixin"></i>
                            <div class="contact-item-content">
                                <h4>微信公众号</h4>
                                <p>云洲说yunzhoushuo</p>
                            </div>
                        </div>
                    </div>
                    
                    <div class="social-links">
                        <a href="#" class="social-link"><i class="fab fa-linkedin-in"></i></a>
                        <a href="#" class="social-link"><i class="fab fa-weixin"></i></a>
                        <a href="#" class="social-link"><i class="fab fa-github"></i></a>
                        <a href="#" class="social-link"><i class="fab fa-medium-m"></i></a>
                    </div>
                </div>
                
                <div class="qrcode-section">
                    <div class="qrcode">
                        <i class="fas fa-qrcode"></i>
                    </div>
                    <p class="qrcode-label">个人公众号：shenwansan2008</p>
                </div>
            </div>
        </div>
    </section>

    <!-- 页脚 -->
    <footer>
        <div class="container">
            <p>&copy; 2025 王伟（云洲） | 版权所有</p>
            <p>基于简历信息创建的个人网站 | 设计：现代简约风格</p>
        </div>
    </footer>

    <script>
        // 移动端菜单切换
        const menuToggle = document.getElementById('menuToggle');
        const navLinks = document.getElementById('navLinks');
        
        menuToggle.addEventListener('click', () => {
            navLinks.classList.toggle('active');
        });
        
        // 平滑滚动
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                
                const target = document.querySelector(this.getAttribute('href'));
                
                window.scrollTo({
                    top: target.offsetTop - 80,
                    behavior: 'smooth'
                });
                
                // 移动端点击后关闭菜单
                if (navLinks.classList.contains('active')) {
                    navLinks.classList.remove('active');
                }
            });
        });
        
        // 滚动时添加导航栏效果
        window.addEventListener('scroll', () => {
            const header = document.querySelector('header');
            if (window.scrollY > 100) {
                header.style.boxShadow = '0 2px 10px rgba(0,0,0,0.2)';
            } else {
                header.style.boxShadow = '0 2px 10px rgba(0,0,0,0.1)';
            }
        });
    </script>
</body>
</html>
