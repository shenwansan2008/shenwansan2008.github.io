<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>王伟（云洲）- 金融科技运营专家</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Noto+Sans+SC:wght@300;400;500;700&family=Roboto:wght@300;400;500;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary-color: #0a192f;
            --secondary-color: #00b4d8;
            --accent-color: #64ffda;
            --light-color: #ccd6f6;
            --dark-color: #020c1b;
            --background-color: #f8f9fa;
            --card-color: #ffffff;
            --text-dark: #333;
            --text-light: #666;
            --transition: all 0.3s ease;
            --shadow: 0 5px 15px rgba(0, 0, 0, 0.08);
            --border-radius: 10px;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Noto Sans SC', 'Roboto', sans-serif;
            color: var(--text-dark);
            background-color: var(--background-color);
            line-height: 1.6;
            overflow-x: hidden;
            scroll-behavior: smooth;
        }

        a {
            text-decoration: none;
            color: var(--secondary-color);
            transition: var(--transition);
        }

        a:hover {
            color: var(--accent-color);
        }

        .container {
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Header & Navigation */
        header {
            background-color: rgba(10, 25, 47, 0.95);
            backdrop-filter: blur(10px);
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            box-shadow: var(--shadow);
            transition: var(--transition);
        }

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 20px;
        }

        .logo {
            font-size: 1.8rem;
            font-weight: 700;
            color: var(--accent-color);
        }

        .nav-links {
            display: flex;
            list-style: none;
        }

        .nav-links li {
            margin-left: 25px;
        }

        .nav-links a {
            color: var(--light-color);
            font-weight: 500;
            position: relative;
            padding: 5px 0;
        }

        .nav-links a:after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 0;
            height: 2px;
            background: var(--accent-color);
            transition: var(--transition);
        }

        .nav-links a:hover:after,
        .nav-links a.active:after {
            width: 100%;
        }

        .hamburger {
            display: none;
            cursor: pointer;
        }

        .hamburger div {
            width: 25px;
            height: 3px;
            background-color: var(--light-color);
            margin: 5px;
            transition: var(--transition);
        }

        /* Hero Section */
        .hero {
            height: 100vh;
            background: linear-gradient(135deg, var(--primary-color) 0%, var(--dark-color) 100%);
            display: flex;
            align-items: center;
            padding-top: 70px;
            position: relative;
            overflow: hidden;
        }

        .hero-content {
            display: flex;
            align-items: center;
            justify-content: space-between;
            width: 100%;
            color: var(--light-color);
            padding: 0 20px;
        }

        .hero-text {
            max-width: 600px;
            z-index: 2;
        }

        .hero-title {
            font-size: 3.5rem;
            font-weight: 700;
            margin-bottom: 20px;
            line-height: 1.2;
        }

        .hero-subtitle {
            font-size: 1.5rem;
            font-weight: 400;
            color: var(--accent-color);
            margin-bottom: 30px;
        }

        .hero-description {
            font-size: 1.1rem;
            margin-bottom: 40px;
            max-width: 550px;
        }

        .hero-image {
            position: relative;
            z-index: 1;
        }

        .profile-img {
            width: 350px;
            height: 350px;
            border-radius: 50%;
            border: 5px solid var(--accent-color);
            object-fit: cover;
            box-shadow: 0 0 40px rgba(100, 255, 218, 0.3);
        }

        .hero-bg {
            position: absolute;
            top: 0;
            right: 0;
            width: 60%;
            height: 100%;
            background: radial-gradient(circle, rgba(0, 180, 216, 0.1) 0%, rgba(10, 25, 47, 0) 70%);
            z-index: 0;
        }

        .tech-pattern {
            position: absolute;
            bottom: 0;
            left: 0;
            width: 100%;
            height: 100px;
            background-image: 
                linear-gradient(to right, rgba(100, 255, 218, 0.1) 1px, transparent 1px),
                linear-gradient(to bottom, rgba(100, 255, 218, 0.1) 1px, transparent 1px);
            background-size: 30px 30px;
            opacity: 0.3;
        }

        /* Section Styling */
        section {
            padding: 100px 0;
        }

        .section-title {
            text-align: center;
            margin-bottom: 60px;
            position: relative;
        }

        .section-title h2 {
            font-size: 2.5rem;
            color: var(--primary-color);
            display: inline-block;
            margin-bottom: 15px;
        }

        .section-title:after {
            content: '';
            position: absolute;
            width: 80px;
            height: 4px;
            background: var(--accent-color);
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            border-radius: 2px;
        }

        .section-subtitle {
            text-align: center;
            color: var(--text-light);
            max-width: 700px;
            margin: 0 auto 50px;
            font-size: 1.1rem;
        }

        /* Card Styling */
        .card {
            background-color: var(--card-color);
            border-radius: var(--border-radius);
            box-shadow: var(--shadow);
            padding: 30px;
            margin-bottom: 30px;
            transition: var(--transition);
            border-left: 4px solid var(--accent-color);
        }

        .card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.1);
        }

        .card-title {
            font-size: 1.5rem;
            color: var(--primary-color);
            margin-bottom: 15px;
            display: flex;
            align-items: center;
        }

        .card-title i {
            margin-right: 10px;
            color: var(--secondary-color);
        }

        .card-subtitle {
            color: var(--secondary-color);
            font-weight: 500;
            margin-bottom: 15px;
            display: block;
        }

        .card-content {
            color: var(--text-light);
        }

        /* Education Section */
        .education-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }

        .education-item {
            position: relative;
            padding-left: 30px;
        }

        .education-item:before {
            content: '';
            position: absolute;
            left: 0;
            top: 10px;
            width: 15px;
            height: 15px;
            border-radius: 50%;
            background: var(--accent-color);
        }

        .education-item:after {
            content: '';
            position: absolute;
            left: 7px;
            top: 25px;
            bottom: -15px;
            width: 1px;
            background: var(--secondary-color);
        }

        .education-item:last-child:after {
            display: none;
        }

        .edu-title {
            font-size: 1.3rem;
            margin-bottom: 5px;
        }

        .edu-major {
            font-weight: 500;
            color: var(--secondary-color);
            margin-bottom: 10px;
        }

        .edu-details {
            color: var(--text-light);
            margin-bottom: 5px;
        }

        /* Skills Section */
        .skills-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }

        .skill-category {
            background: linear-gradient(145deg, #ffffff, #f0f0f0);
            border-radius: var(--border-radius);
            box-shadow: var(--shadow);
            padding: 30px;
            transition: var(--transition);
        }

        .skill-category:hover {
            transform: translateY(-5px);
        }

        .skill-category h3 {
            font-size: 1.5rem;
            color: var(--primary-color);
            margin-bottom: 20px;
            display: flex;
            align-items: center;
        }

        .skill-category h3 i {
            margin-right: 10px;
            color: var(--accent-color);
        }

        .skill-item {
            margin-bottom: 20px;
            position: relative;
            padding-left: 30px;
        }

        .skill-item:before {
            content: '✓';
            position: absolute;
            left: 0;
            top: 0;
            color: var(--accent-color);
            font-weight: bold;
        }

        /* Experience Section */
        .timeline {
            position: relative;
            max-width: 800px;
            margin: 0 auto;
        }

        .timeline:before {
            content: '';
            position: absolute;
            top: 0;
            bottom: 0;
            width: 2px;
            background: var(--secondary-color);
            left: 50%;
            margin-left: -1px;
        }

        .timeline-item {
            margin-bottom: 50px;
            position: relative;
            width: 100%;
        }

        .timeline-item:nth-child(odd) .timeline-content {
            margin-left: auto;
            margin-right: calc(50% + 30px);
            text-align: right;
        }

        .timeline-item:nth-child(even) .timeline-content {
            margin-left: calc(50% + 30px);
        }

        .timeline-icon {
            position: absolute;
            left: 50%;
            top: 0;
            width: 50px;
            height: 50px;
            background: var(--primary-color);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            margin-left: -25px;
            z-index: 2;
            box-shadow: 0 0 0 5px rgba(0, 180, 216, 0.3);
        }

        .timeline-content {
            background: var(--card-color);
            padding: 30px;
            border-radius: var(--border-radius);
            box-shadow: var(--shadow);
            width: calc(50% - 30px);
        }

        .company {
            color: var(--secondary-color);
            font-weight: 600;
            margin-bottom: 10px;
        }

        .position {
            font-weight: 700;
            margin-bottom: 15px;
            font-size: 1.3rem;
        }

        .date {
            color: var(--text-light);
            margin-bottom: 15px;
            display: block;
        }

        .responsibilities {
            margin-top: 15px;
        }

        .responsibilities li {
            margin-bottom: 8px;
            position: relative;
            padding-left: 20px;
        }

        .responsibilities li:before {
            content: '•';
            position: absolute;
            left: 0;
            color: var(--accent-color);
        }

        /* Projects Section */
        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }

        .project-card {
            background: var(--card-color);
            border-radius: var(--border-radius);
            overflow: hidden;
            box-shadow: var(--shadow);
            transition: var(--transition);
        }

        .project-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.15);
        }

        .project-header {
            background: linear-gradient(135deg, var(--primary-color) 0%, var(--dark-color) 100%);
            color: white;
            padding: 20px;
        }

        .project-title {
            font-size: 1.3rem;
            margin-bottom: 5px;
        }

        .project-category {
            color: var(--accent-color);
            font-size: 0.9rem;
        }

        .project-body {
            padding: 20px;
        }

        .project-description {
            color: var(--text-light);
            margin-bottom: 15px;
        }

        .project-stats {
            display: flex;
            justify-content: space-between;
            background: rgba(100, 255, 218, 0.1);
            padding: 10px 15px;
            border-radius: 5px;
            margin-top: 15px;
            font-size: 0.9rem;
        }

        .stat {
            text-align: center;
        }

        .stat-value {
            font-weight: 700;
            color: var(--primary-color);
            font-size: 1.1rem;
        }

        .stat-label {
            color: var(--text-light);
            font-size: 0.8rem;
        }

        /* Certificates Section */
        .certificates-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
        }

        .certificate-card {
            background: var(--card-color);
            border-radius: var(--border-radius);
            padding: 25px;
            text-align: center;
            box-shadow: var(--shadow);
            transition: var(--transition);
            border-top: 3px solid var(--accent-color);
        }

        .certificate-card:hover {
            transform: translateY(-5px);
        }

        .certificate-icon {
            font-size: 3rem;
            color: var(--secondary-color);
            margin-bottom: 15px;
        }

        .certificate-title {
            font-size: 1.1rem;
            margin-bottom: 10px;
            font-weight: 600;
        }

        .certificate-org {
            color: var(--text-light);
            font-size: 0.9rem;
        }

        /* Contact Section */
        .contact {
            background: linear-gradient(135deg, var(--primary-color) 0%, var(--dark-color) 100%);
            color: var(--light-color);
            text-align: center;
        }

        .contact .section-title h2 {
            color: white;
        }

        .contact-info {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
            max-width: 800px;
            margin: 0 auto 50px;
        }

        .contact-item {
            padding: 30px;
            background: rgba(255, 255, 255, 0.08);
            border-radius: var(--border-radius);
            transition: var(--transition);
        }

        .contact-item:hover {
            background: rgba(255, 255, 255, 0.12);
            transform: translateY(-5px);
        }

        .contact-icon {
            font-size: 2.5rem;
            color: var(--accent-color);
            margin-bottom: 20px;
        }

        .contact-title {
            font-size: 1.2rem;
            margin-bottom: 10px;
        }

        .contact-detail {
            font-size: 1.1rem;
        }

        .qr-code {
            max-width: 200px;
            margin: 30px auto;
            border: 5px solid white;
            border-radius: 10px;
            overflow: hidden;
        }

        .qr-code img {
            width: 100%;
            display: block;
        }

        .footer {
            background: var(--dark-color);
            color: var(--light-color);
            text-align: center;
            padding: 20px;
            font-size: 0.9rem;
        }

        /* Responsive Design */
        @media (max-width: 992px) {
            .hero-content {
                flex-direction: column;
                text-align: center;
                padding-top: 50px;
            }
            
            .hero-text {
                margin-bottom: 50px;
            }
            
            .hero-title {
                font-size: 2.8rem;
            }
            
            .hero-subtitle {
                font-size: 1.3rem;
            }
            
            .profile-img {
                width: 280px;
                height: 280px;
            }
            
            .timeline:before {
                left: 30px;
            }
            
            .timeline-item:nth-child(odd) .timeline-content,
            .timeline-item:nth-child(even) .timeline-content {
                margin-left: 70px;
                margin-right: 0;
                text-align: left;
            }
            
            .timeline-icon {
                left: 30px;
            }
        }

        @media (max-width: 768px) {
            .hamburger {
                display: block;
            }
            
            .nav-links {
                position: absolute;
                top: 70px;
                right: 0;
                background: var(--primary-color);
                width: 100%;
                height: 0;
                flex-direction: column;
                align-items: center;
                overflow: hidden;
                transition: var(--transition);
            }
            
            .nav-links.active {
                height: 300px;
                padding: 20px 0;
            }
            
            .nav-links li {
                margin: 15px 0;
                opacity: 0;
                transform: translateX(20px);
                transition: var(--transition);
            }
            
            .nav-links.active li {
                opacity: 1;
                transform: translateX(0);
            }
            
            .hero-title {
                font-size: 2.3rem;
            }
            
            .section-title h2 {
                font-size: 2rem;
            }
        }

        @media (max-width: 576px) {
            .hero-title {
                font-size: 2rem;
            }
            
            .hero-subtitle {
                font-size: 1.1rem;
            }
            
            .profile-img {
                width: 220px;
                height: 220px;
            }
            
            .card, .timeline-content {
                padding: 20px;
            }
            
            .timeline-icon {
                width: 40px;
                height: 40px;
                margin-left: -20px;
            }
        }
    </style>
</head>
<body>
    <!-- Header & Navigation -->
    <header>
        <nav>
            <div class="logo">王伟（云洲）</div>
            <ul class="nav-links">
                <li><a href="#education" class="nav-link">教育背景</a></li>
                <li><a href="#skills" class="nav-link">技能特长</a></li>
                <li><a href="#experience" class="nav-link">工作经历</a></li>
                <li><a href="#projects" class="nav-link">项目经历</a></li>
                <li><a href="#certificates" class="nav-link">证书资质</a></li>
                <li><a href="#contact" class="nav-link">联系方式</a></li>
            </ul>
            <div class="hamburger">
                <div class="line1"></div>
                <div class="line2"></div>
                <div class="line3"></div>
            </div>
        </nav>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <div class="hero-bg"></div>
        <div class="tech-pattern"></div>
        <div class="container hero-content">
            <div class="hero-text">
                <h1 class="hero-title">互联网金融运营总监</h1>
                <h2 class="hero-subtitle">前阿里巴巴/蚂蚁集团资深产品运营专家</h2>
                <p class="hero-description">
                    南大硕士，10年+金融科技/O2O电商背景，2家上市公司及一线大厂产品运营经验。拥有体系化的产品运营管理方法论，擅长用户增长运营、产品运营、流量运营、团队及项目管理。
                </p>
                <div class="hero-buttons">
                    <a href="#contact" class="btn">联系我 </a>
                    <a href="#projects" class="btn"> 查看项目</a>
                </div>
            </div>
            <div class="hero-image">
                <img src="https://s21.ax1x.com/2025/06/15/pVAqWF0.jpg" alt="王伟" class="profile-img">
            </div>
        </div>
    </section>

    <!-- Education Section -->
    <section id="education">
        <div class="container">
            <div class="section-title">
                <h2>教育背景</h2>
            </div>
            <div class="education-grid">
                <div class="education-item">
                    <h3 class="edu-title">南京大学（985）</h3>
                    <div class="edu-major">信息管理学院 · 数字出版专业</div>
                    <div class="edu-date">2011.09 - 2014.06</div>
                    <p class="edu-details">班长/研会主席，2013国家奖学金，优秀毕业生</p>
                </div>
                <div class="education-item">
                    <h3 class="edu-title">安徽大学（211）</h3>
                    <div class="edu-major">汉语言文学（辅修工商管理）</div>
                    <div class="edu-date">2003.10 - 2007.06</div>
                    <p class="edu-details">学生会部长，安徽大学优秀毕业生</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Skills Section -->
    <section id="skills" style="background-color: #f0f5ff;">
        <div class="container">
            <div class="section-title">
                <h2>技能特长</h2>
            </div>
            <div class="skills-container">
                <div class="skill-category">
                    <h3><i class="fas fa-users"></i> 用户运营</h3>
                    <div class="skill-item">具备亿级用户体量平台的运营经验</div>
                    <div class="skill-item">擅长用户生命周期管理及分层运营</div>
                    <div class="skill-item">精通活动策划及运营、数据运营</div>
                    <div class="skill-item">擅长精准营销触达及转化率提升</div>
                    <div class="skill-item">C类/B类小微/KA客户全类型覆盖</div>
                </div>
                <div class="skill-category">
                    <h3><i class="fas fa-laptop-code"></i> 产品运营</h3>
                    <div class="skill-item">擅长APP运营/活动运营/流量运营</div>
                    <div class="skill-item">精通看板/标签/营销工具产品运营</div>
                    <div class="skill-item">熟练使用Axure/XMind/ProcessOn</div>
                    <div class="skill-item">掌握Python/SQL/Excel等BI工具</div>
                    <div class="skill-item">用户洞察/需求策划/AB测试专家</div>
                </div>
                <div class="skill-category">
                    <h3><i class="fas fa-chart-line"></i> 内容/流量运营</h3>
                    <div class="skill-item">流量精细化运营及渠道投放专家</div>
                    <div class="skill-item">精通新媒体运营及公私域流量整合</div>
                    <div class="skill-item">熟悉主流数字营销系统及工具</div>
                    <div class="skill-item">人人都是产品经理专栏作家</div>
                    <div class="skill-item">公众号"云洲说"主理人</div>
                </div>
                <div class="skill-category">
                    <h3><i class="fas fa-tasks"></i> 项目及团队管理</h3>
                    <div class="skill-item">中型项目及团队管理能力</div>
                    <div class="skill-item">擅长业务策略拆解及团队分工</div>
                    <div class="skill-item">统筹风控/产品/法务/技术团队</div>
                    <div class="skill-item">从0到1及从1到100项目经验</div>
                    <div class="skill-item">算法模型/AI赋能/银行合规项目</div>
                </div>
            </div>
        </div>
    </section>

    <!-- Experience Section -->
    <section id="experience">
        <div class="container">
            <div class="section-title">
                <h2>工作经历</h2>
            </div>
            <div class="timeline">
                <!-- Experience 1 -->
                <div class="timeline-item">
                    <div class="timeline-icon">
                        <i class="fas fa-bank"></i>
                    </div>
                    <div class="timeline-content">
                        <div class="company">苏宁银行</div>
                        <h3 class="position">普惠金融客群运营部 · 产品运营总监</h3>
                        <div class="date">2024年7月 - 2025年2月</div>
                        <p class="card-content">小微客群互联网信贷业务，核心KPI为信贷业务规模、用户数及活跃度（汇报对象：董事长、副行）</p>
                        <ul class="responsibilities">
                            <li>搭建运营团队及用户增长体系，制订团队业务指标</li>
                            <li>跨部门组建全行互联网运营项目组，提升运营水平</li>
                            <li>搭建体系化运营管户策略，统筹公域/私域/外部流量</li>
                            <li>公众号/视频号新媒体运营阵地建设，行业TOP5</li>
                            <li>主导AI工具应用提效、智能外呼机器人接入</li>
                        </ul>
                    </div>
                </div>
                
                <!-- Experience 2 -->
                <div class="timeline-item">
                    <div class="timeline-icon">
                        <i class="fab fa-alipay"></i>
                    </div>
                    <div class="timeline-content">
                        <div class="company">蚂蚁集团/阿里巴巴</div>
                        <h3 class="position">网商银行/本地生活 · 产品运营专家</h3>
                        <div class="date">2020年1月 - 2024年5月</div>
                        <p class="card-content">互金产品及O2O本地电商运营，聚焦用户数及业务量增长（汇报对象：行长、业务线负责人）</p>
                        <ul class="responsibilities">
                            <li>本地生活O2O业务运营（职级P8）</li>
                            <li>基于用户分层进行精准人群构建与营销转化</li>
                            <li>支付宝/饿了么平台SAAS运营，链接B端与C端</li>
                            <li>信贷产品客群线上运营（小微、电商、三农客户）</li>
                            <li>策划支付宝集五福/双11大促等大型活动</li>
                            <li>获网商银行2022年优秀员工称号</li>
                        </ul>
                    </div>
                </div>
                
                <!-- Experience 3 -->
                <div class="timeline-item">
                    <div class="timeline-icon">
                        <i class="fas fa-credit-card"></i>
                    </div>
                    <div class="timeline-content">
                        <div class="company">51信用卡</div>
                        <h3 class="position">理财业务部 · 产品运营经理</h3>
                        <div class="date">2017年4月 - 2019年12月</div>
                        <p class="card-content">To C个人理财类产品，核心KPI为APP用户及资金营收规模增长（汇报对象：业务线负责人）</p>
                        <ul class="responsibilities">
                            <li>构建生命周期运营体系（新手/成长/裂变/召回）</li>
                            <li>推动开发票券/活动模板/标签库等运营工具</li>
                            <li>策划"51信用卡五周年庆"活动，带来5.5亿元净充值</li>
                            <li>统筹搭建理财用户增长运营体系</li>
                            <li>洽谈接入平安、百信等10多家机构理财产品</li>
                        </ul>
                    </div>
                </div>
                
                <!-- Experience 4 -->
                <div class="timeline-item">
                    <div class="timeline-icon">
                        <i class="fas fa-chart-bar"></i>
                    </div>
                    <div class="timeline-content">
                        <div class="company">东方财富</div>
                        <h3 class="position">个人产品部 · 用户运营/营销策划</h3>
                        <div class="date">2014年7月 - 2017年4月</div>
                        <p class="card-content">财经资讯及证券交易服务，核心目标为APP注册用户及证券开户数增长（汇报对象：业务线负责人）</p>
                        <ul class="responsibilities">
                            <li>制订用户增长运营计划，策划项目/活动方案</li>
                            <li>策划东方财富实盘炒股大赛等30+活动</li>
                            <li>优化产品及项目流程，提升用户体验</li>
                            <li>输出产品需求文档182次，担任项目PM</li>
                            <li>跟踪平安证券、同花顺等竞品动态</li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects" style="background-color: #f0f5ff;">
        <div class="container">
            <div class="section-title">
                <h2>代表项目</h2>
            </div>
            <div class="projects-grid">
                <!-- Project 1 -->
                <div class="project-card">
                    <div class="project-header">
                        <h3 class="project-title">51信用卡-人品专家</h3>
                        <div class="project-category">裂变增长 · 用户运营</div>
                    </div>
                    <div class="project-body">
                        <p class="project-description">通过用户MGM分享裂变机制设计，从0到1构建用户增长裂变模块</p>
                        <div class="project-stats">
                            <div class="stat">
                                <div class="stat-value">33%+</div>
                                <div class="stat-label">平台新用户占比</div>
                            </div>
                        </div>
                    </div>
                </div>
                
                <!-- Project 2 -->
                <div class="project-card">
                    <div class="project-header">
                        <h3 class="project-title">支付宝＆KFC联名会员</h3>
                        <div class="project-category">精准营销 · 会员运营</div>
                    </div>
                    <div class="project-body">
                        <p class="project-description">通过阿里巴巴-本地生活CRM精准营销运营，实现高效会员转化</p>
                        <div class="project-stats">
                            <div class="stat">
                                <div class="stat-value">50,000+</div>
                                <div class="stat-label">单日转化新客</div>
                            </div>
                        </div>
                    </div>
                </div>
                
                <!-- Project 3 -->
                <div class="project-card">
                    <div class="project-header">
                        <h3 class="project-title">网商银行2021丰收节</h3>
                        <div class="project-category">活动运营 · 金融科技</div>
                    </div>
                    <div class="project-body">
                        <p class="project-description">针对性策划节点营销活动，借助支付宝流量触达客户</p>
                        <div class="project-stats">
                            <div class="stat">
                                <div class="stat-value">80,000+</div>
                                <div class="stat-label">转化客户数</div>
                            </div>
                            <div class="stat">
                                <div class="stat-value">25亿+</div>
                                <div class="stat-label">信贷支用金额</div>
                            </div>
                        </div>
                    </div>
                </div>
                
                <!-- Project 4 -->
                <div class="project-card">
                    <div class="project-header">
                        <h3 class="project-title">全国县域评级模型</h3>
                        <div class="project-category">算法模型 · 风控系统</div>
                    </div>
                    <div class="project-body">
                        <p class="project-description">基于支付宝及外部数据训练模型，实现全国县域中宏观评级</p>
                        <div class="project-stats">
                            <div class="stat">
                                <div class="stat-value">120亿+</div>
                                <div class="stat-label">业务增益</div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Certificates Section -->
    <section id="certificates">
        <div class="container">
            <div class="section-title">
                <h2>证书资质</h2>
            </div>
            <div class="certificates-container">
                <div class="certificate-card">
                    <div class="certificate-icon">
                        <i class="fas fa-file-invoice-dollar"></i>
                    </div>
                    <h3 class="certificate-title">金融相关资质</h3>
                    <p class="certificate-org">基金/证券/银行从业资格</p>
                    <p class="certificate-org">中级经济师（金融）</p>
                </div>
                
                <div class="certificate-card">
                    <div class="certificate-icon">
                        <i class="fas fa-laptop-code"></i>
                    </div>
                    <h3 class="certificate-title">互联网相关</h3>
                    <p class="certificate-org">PCEP国际Python程序员认证</p>
                    <p class="certificate-org">CAIP人工智能职场应用师</p>
                </div>
                
                <div class="certificate-card">
                    <div class="certificate-icon">
                        <i class="fas fa-cogs"></i>
                    </div>
                    <h3 class="certificate-title">发明专利</h3>
                    <p class="certificate-org">个体属性挂载及群体属性分层大数据授信应用装置</p>
                    <p class="certificate-org">专利号CN117709963A</p>
                </div>
                
                <div class="certificate-card">
                    <div class="certificate-icon">
                        <i class="fas fa-graduation-cap"></i>
                    </div>
                    <h3 class="certificate-title">培训认证</h3>
                    <p class="certificate-org">腾讯课堂"互金产品设计提升班"</p>
                    <p class="certificate-org">腾讯＆起点学院运营总监培训</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="contact">
        <div class="container">
            <div class="section-title">
                <h2>联系方式</h2>
            </div>
            <div class="contact-info">
                <div class="contact-item">
                    <div class="contact-icon">
                        <i class="fas fa-phone-alt"></i>
                    </div>
                    <h3 class="contact-title">电话</h3>
                    <p class="contact-detail">18557519167</p>
                </div>
                
                <div class="contact-item">
                    <div class="contact-icon">
                        <i class="fas fa-envelope"></i>
                    </div>
                    <h3 class="contact-title">邮箱</h3>
                    <p class="contact-detail">shenwansan2008@163.com</p>
                </div>
                
                <div class="contact-item">
                    <div class="contact-icon">
                        <i class="fas fa-map-marker-alt"></i>
                    </div>
                    <h3 class="contact-title">所在地</h3>
                    <p class="contact-detail">浙江 · 杭州</p>
                </div>
            </div>
            
            <div class="contact-item">
                <div class="contact-icon">
                    <i class="fab fa-weixin"></i>
                </div>
                <h3 class="contact-title">公众号</h3>
                <p class="contact-detail">云洲说（专注互联网、金融科技）</p>
                <div class="qr-code">
                    <img src="https://23qn.f2z.cn/srnKSt" alt="公众号二维码">
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="footer">
        <div class="container">
            <p>© 2025 王伟（云洲）- 金融科技产品运营专家 | 公众号“云洲说”主理人 | 杭州高层次人才</p>
            <p>本网站仅用于个人展示，保留所有权利</p>
        </div>
    </footer>

    <script>
        // Navigation scroll effect
        window.addEventListener('scroll', function() {
            const header = document.querySelector('header');
            if (window.scrollY > 50) {
                header.style.boxShadow = '0 5px 20px rgba(0, 0, 0, 0.1)';
                header.style.background = 'rgba(10, 25, 47, 0.98)';
            } else {
                header.style.boxShadow = 'none';
                header.style.background = 'rgba(10, 25, 47, 0.95)';
            }
        });

        // Mobile menu toggle
        const hamburger = document.querySelector('.hamburger');
        const navLinks = document.querySelector('.nav-links');
        
        hamburger.addEventListener('click', function() {
            navLinks.classList.toggle('active');
            hamburger.classList.toggle('active');
        });

        // Close mobile menu when clicking a link
        const navItems = document.querySelectorAll('.nav-link');
        navItems.forEach(item => {
            item.addEventListener('click', function() {
                navLinks.classList.remove('active');
                hamburger.classList.remove('active');
            });
        });

        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    window.scrollTo({
                        top: target.offsetTop - 70,
                        behavior: 'smooth'
                    });
                }
            });
        });
    </script>
</body>
</html>
