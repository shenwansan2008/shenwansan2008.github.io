<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>王伟（云洲）- 互联网金融产品运营专家</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary: #0a192f; /* 深蓝色主色调 */
            --secondary: #64ffda; /* 科技绿强调色 */
            --accent: #112240; /* 深蓝色辅助色 */
            --light: #ccd6f6; /* 浅色文字 */
            --dark: #020c1b; /* 深色背景 */
            --gray: #8892b0; /* 灰色文字 */
            --card-bg: rgba(10, 25, 47, 0.8); /* 卡片背景 */
            --transition: all 0.3s ease;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, var(--dark) 0%, var(--primary) 100%);
            color: var(--light);
            line-height: 1.6;
            overflow-x: hidden;
            position: relative;
        }
        
        body::before {
            content: "";
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: 
                radial-gradient(circle at 10% 20%, rgba(100, 255, 218, 0.1) 0%, transparent 20%),
                radial-gradient(circle at 90% 80%, rgba(100, 255, 218, 0.1) 0%, transparent 20%),
                radial-gradient(circle at 50% 50%, rgba(100, 255, 218, 0.05) 0%, transparent 40%);
            z-index: -1;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* 头部样式 */
        header {
            padding: 40px 0;
            text-align: center;
            position: relative;
            background: rgba(10, 25, 47, 0.7);
            backdrop-filter: blur(10px);
            border-bottom: 1px solid rgba(100, 255, 218, 0.2);
        }
        
        .profile-container {
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 20px;
        }
        
        .profile-img {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            border: 3px solid var(--secondary);
            overflow: hidden;
            box-shadow: 0 0 30px rgba(100, 255, 218, 0.3);
            transition: var(--transition);
        }
        
        .profile-img:hover {
            transform: scale(1.05);
            box-shadow: 0 0 40px rgba(100, 255, 218, 0.5);
        }
        
        .profile-img img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
        
        .header-content {
            max-width: 800px;
        }
        
        h1 {
            font-size: 2.5rem;
            margin-bottom: 10px;
            background: linear-gradient(90deg, var(--light), var(--secondary));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            text-shadow: 0 2px 10px rgba(100, 255, 218, 0.2);
        }
        
        .title {
            font-size: 1.4rem;
            color: var(--secondary);
            margin-bottom: 20px;
            font-weight: 500;
        }
        
        .contact-info {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 25px;
            margin-top: 20px;
        }
        
        .contact-item {
            display: flex;
            align-items: center;
            gap: 8px;
            font-size: 1.1rem;
        }
        
        .contact-item i {
            color: var(--secondary);
        }
        
        /* 内容部分样式 */
        section {
            padding: 60px 0;
            border-bottom: 1px solid rgba(100, 255, 218, 0.1);
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 50px;
            position: relative;
        }
        
        .section-title h2 {
            font-size: 2.2rem;
            display: inline-block;
            padding-bottom: 10px;
            position: relative;
        }
        
        .section-title h2::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 3px;
            background: var(--secondary);
            border-radius: 3px;
        }
        
        /* 教育背景 */
        .education {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 30px;
            margin-top: 30px;
        }
        
        .edu-item {
            background: var(--card-bg);
            border: 1px solid rgba(100, 255, 218, 0.1);
            border-radius: 10px;
            padding: 25px;
            width: 100%;
            max-width: 500px;
            transition: var(--transition);
            box-shadow: 0 10px 30px rgba(2, 12, 27, 0.5);
        }
        
        .edu-item:hover {
            transform: translateY(-5px);
            border-color: var(--secondary);
        }
        
        .edu-header {
            display: flex;
            justify-content: space-between;
            margin-bottom: 15px;
            align-items: center;
        }
        
        .edu-school {
            font-size: 1.4rem;
            font-weight: 600;
            color: var(--secondary);
        }
        
        .edu-period {
            background: rgba(100, 255, 218, 0.1);
            padding: 5px 12px;
            border-radius: 20px;
            font-size: 0.9rem;
        }
        
        .edu-major {
            font-size: 1.2rem;
            margin-bottom: 15px;
            color: var(--light);
        }
        
        .edu-desc {
            color: var(--gray);
            font-size: 1rem;
        }
        
        /* 技能特长 */
        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .skill-card {
            background: var(--card-bg);
            border-radius: 10px;
            padding: 30px;
            border: 1px solid rgba(100, 255, 218, 0.1);
            transition: var(--transition);
            box-shadow: 0 10px 30px rgba(2, 12, 27, 0.5);
        }
        
        .skill-card:hover {
            transform: translateY(-5px);
            border-color: var(--secondary);
        }
        
        .skill-card h3 {
            color: var(--secondary);
            font-size: 1.5rem;
            margin-bottom: 20px;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .skill-card h3 i {
            font-size: 1.8rem;
        }
        
        .skill-list {
            list-style-type: none;
        }
        
        .skill-list li {
            margin-bottom: 15px;
            padding-left: 30px;
            position: relative;
        }
        
        .skill-list li::before {
            content: '✓';
            position: absolute;
            left: 0;
            color: var(--secondary);
            font-weight: bold;
        }
        
        /* 工作经历 */
        .timeline {
            position: relative;
            max-width: 900px;
            margin: 0 auto;
        }
        
        .timeline::before {
            content: '';
            position: absolute;
            top: 0;
            bottom: 0;
            width: 2px;
            background: var(--secondary);
            left: 50%;
            margin-left: -1px;
        }
        
        .timeline-item {
            margin-bottom: 50px;
            position: relative;
        }
        
        .timeline-content {
            background: var(--card-bg);
            border: 1px solid rgba(100, 255, 218, 0.1);
            border-radius: 10px;
            padding: 30px;
            width: calc(50% - 40px);
            position: relative;
            box-shadow: 0 10px 30px rgba(2, 12, 27, 0.5);
            transition: var(--transition);
        }
        
        .timeline-content:hover {
            transform: translateY(-5px);
            border-color: var(--secondary);
        }
        
        .timeline-item:nth-child(odd) .timeline-content {
            left: 0;
        }
        
        .timeline-item:nth-child(even) .timeline-content {
            left: calc(50% + 40px);
        }
        
        .timeline-period {
            position: absolute;
            top: 20px;
            width: 120px;
            text-align: center;
            padding: 8px;
            background: var(--secondary);
            color: var(--dark);
            font-weight: 600;
            border-radius: 20px;
            font-size: 0.9rem;
        }
        
        .timeline-item:nth-child(odd) .timeline-period {
            right: -160px;
        }
        
        .timeline-item:nth-child(even) .timeline-period {
            left: -160px;
        }
        
        .company {
            display: flex;
            align-items: center;
            gap: 15px;
            margin-bottom: 15px;
        }
        
        .company-logo {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            background: var(--accent);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.5rem;
            color: var(--secondary);
        }
        
        .company-info h3 {
            font-size: 1.5rem;
            color: var(--light);
        }
        
        .company-info .position {
            color: var(--secondary);
            font-size: 1.1rem;
        }
        
        .job-desc {
            color: var(--gray);
            margin: 20px 0;
            font-size: 1rem;
        }
        
        .achievements {
            margin-top: 20px;
        }
        
        .achievements h4 {
            color: var(--secondary);
            margin-bottom: 10px;
            font-size: 1.2rem;
        }
        
        .achievements ul {
            list-style-type: none;
            padding-left: 20px;
        }
        
        .achievements li {
            margin-bottom: 10px;
            position: relative;
            padding-left: 20px;
        }
        
        .achievements li::before {
            content: '•';
            position: absolute;
            left: 0;
            color: var(--secondary);
            font-size: 1.2rem;
        }
        
        /* 项目经历 */
        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .project-card {
            background: var(--card-bg);
            border-radius: 10px;
            padding: 25px;
            border: 1px solid rgba(100, 255, 218, 0.1);
            transition: var(--transition);
            box-shadow: 0 10px 30px rgba(2, 12, 27, 0.5);
        }
        
        .project-card:hover {
            transform: translateY(-5px);
            border-color: var(--secondary);
        }
        
        .project-card h3 {
            color: var(--secondary);
            font-size: 1.4rem;
            margin-bottom: 15px;
        }
        
        .project-desc {
            color: var(--gray);
            margin-bottom: 20px;
            font-size: 1rem;
        }
        
        .project-stats {
            display: flex;
            gap: 15px;
            flex-wrap: wrap;
        }
        
        .stat-item {
            background: rgba(100, 255, 218, 0.1);
            padding: 8px 15px;
            border-radius: 20px;
            font-size: 0.9rem;
        }
        
        /* 证书资质 */
        .certificates {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 20px;
        }
        
        .cert-card {
            background: var(--card-bg);
            border: 1px solid rgba(100, 255, 218, 0.1);
            border-radius: 10px;
            padding: 20px;
            width: calc(50% - 20px);
            min-width: 300px;
            transition: var(--transition);
            box-shadow: 0 10px 30px rgba(2, 12, 27, 0.5);
        }
        
        .cert-card:hover {
            transform: translateY(-5px);
            border-color: var(--secondary);
        }
        
        .cert-card h3 {
            color: var(--secondary);
            font-size: 1.3rem;
            margin-bottom: 15px;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .cert-list {
            list-style-type: none;
        }
        
        .cert-list li {
            margin-bottom: 10px;
            padding-left: 25px;
            position: relative;
        }
        
        .cert-list li::before {
            content: '✓';
            position: absolute;
            left: 0;
            color: var(--secondary);
            font-weight: bold;
        }
        
        /* 联系方式 */
        .contact-section {
            text-align: center;
            padding-bottom: 80px;
        }
        
        .contact-methods {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 30px;
            margin-top: 40px;
        }
        
        .contact-card {
            background: var(--card-bg);
            border: 1px solid rgba(100, 255, 218, 0.1);
            border-radius: 10px;
            padding: 30px;
            width: 250px;
            transition: var(--transition);
            box-shadow: 0 10px 30px rgba(2, 12, 27, 0.5);
        }
        
        .contact-card:hover {
            transform: translateY(-5px);
            border-color: var(--secondary);
        }
        
        .contact-icon {
            font-size: 2.5rem;
            color: var(--secondary);
            margin-bottom: 20px;
        }
        
        .contact-card h3 {
            font-size: 1.3rem;
            margin-bottom: 10px;
        }
        
        .contact-card p {
            color: var(--gray);
            font-size: 1.1rem;
        }
        
        /* 页脚 */
        footer {
            text-align: center;
            padding: 30px 0;
            color: var(--gray);
            font-size: 0.9rem;
            background: rgba(10, 25, 47, 0.7);
            border-top: 1px solid rgba(100, 255, 218, 0.1);
        }
        
        /* 响应式设计 */
        @media (max-width: 992px) {
            .timeline::before {
                left: 30px;
            }
            
            .timeline-content {
                width: calc(100% - 80px);
                margin-left: 80px;
            }
            
            .timeline-item:nth-child(even) .timeline-content {
                left: 0;
            }
            
            .timeline-period {
                left: -60px !important;
                right: auto !important;
            }
        }
        
        @media (max-width: 768px) {
            h1 {
                font-size: 2rem;
            }
            
            .title {
                font-size: 1.2rem;
            }
            
            .contact-info {
                flex-direction: column;
                gap: 10px;
            }
            
            .section-title h2 {
                font-size: 1.8rem;
            }
            
            .cert-card {
                width: 100%;
            }
            
            .timeline-content {
                width: calc(100% - 40px);
                margin-left: 40px;
            }
            
            .timeline-period {
                left: -40px !important;
            }
        }
        
        @media (max-width: 480px) {
            .profile-img {
                width: 120px;
                height: 120px;
            }
            
            .company {
                flex-direction: column;
                align-items: flex-start;
            }
            
            .company-logo {
                margin-bottom: 10px;
            }
            
            .skills-grid, .projects-grid {
                grid-template-columns: 1fr;
            }
            
            .timeline-content {
                width: 100%;
                margin-left: 0;
            }
            
            .timeline::before {
                display: none;
            }
            
            .timeline-period {
                position: relative;
                left: 0 !important;
                right: 0 !important;
                top: 0;
                margin-bottom: 15px;
            }
        }
    </style>
</head>
<body>
    <!-- 头部区域 -->
    <header>
        <div class="container">
            <div class="profile-container">
                <div class="profile-img">
                    <img src="https://s21.ax1x.com/2025/06/15/pVAqWF0.jpg" alt="王伟">
                </div>
                <div class="header-content">
                    <h1>王伟（云洲）</h1>
                    <div class="title">互联网金融运营总监 | 前大厂资深产品运营专家</div>
                    <p>南大硕士，10年+金融科技/O2O电商行业背景，2家互联网上市公司及一线大厂运营管理经验，杭州高层次人才，拥有体系化产品运营管理方法论</p>
                    
                    <div class="contact-info">
                        <div class="contact-item">
                            <i class="fas fa-phone"></i>
                            <span>18557519167</span>
                        </div>
                        <div class="contact-item">
                            <i class="fas fa-envelope"></i>
                            <span>shenwansan2008@163.com</span>
                        </div>
                        <div class="contact-item">
                            <i class="fab fa-weixin"></i>
                            <span>云洲说</span>
                        </div>
                        <div class="contact-item">
                            <i class="fas fa-map-marker-alt"></i>
                            <span>杭州</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </header>
    
    <main class="container">
        <!-- 教育背景 -->
        <section id="education">
            <div class="section-title">
                <h2>教育背景</h2>
            </div>
            <div class="education">
                <div class="edu-item">
                    <div class="edu-header">
                        <div class="edu-school">南京大学（985）</div>
                        <div class="edu-period">2011.09-2014.06</div>
                    </div>
                    <div class="edu-major">信息管理学院 · 数字出版专业</div>
                    <div class="edu-desc">
                        班长/研会主席，2013国家奖学金，优秀毕业生
                    </div>
                </div>
                
                <div class="edu-item">
                    <div class="edu-header">
                        <div class="edu-school">安徽大学（211）</div>
                        <div class="edu-period">2003.10-2007.06</div>
                    </div>
                    <div class="edu-major">汉语言文学（辅修工商管理）</div>
                    <div class="edu-desc">
                        学生会宣传部部长，安大优秀毕业生
                    </div>
                </div>
            </div>
        </section>
        
        <!-- 技能特长 -->
        <section id="skills">
            <div class="section-title">
                <h2>技能特长</h2>
            </div>
            <div class="skills-grid">
                <div class="skill-card">
                    <h3><i class="fas fa-users"></i> 用户运营</h3>
                    <ul class="skill-list">
                        <li>亿级用户体量平台的运营经验</li>
                        <li>用户生命周期、业务转化漏斗管理</li>
                        <li>用户分层运营、活动策划及运营</li>
                        <li>商家商品运营、数据运营、精准营销触达</li>
                        <li>拉新、促活、GMV转化指标优化</li>
                        <li>覆盖C类、B类小微及行业KA大客户</li>
                    </ul>
                </div>
                
                <div class="skill-card">
                    <h3><i class="fas fa-mobile-alt"></i> 产品运营</h3>
                    <ul class="skill-list">
                        <li>APP迭代/活动运营/流量投放/数据看板</li>
                        <li>标签及营销工具产品运营</li>
                        <li>Axure、XMind、ProcessOn熟练应用</li>
                        <li>Python、SQL、Excel等BI工具</li>
                        <li>用户洞察/需求策划能力</li>
                        <li>用户反馈/指标监测/AB测试驱动迭代</li>
                    </ul>
                </div>
                
                <div class="skill-card">
                    <h3><i class="fas fa-chart-line"></i> 内容/流量运营</h3>
                    <ul class="skill-list">
                        <li>流量精细化运营、渠道投放</li>
                        <li>新媒体运营及策略规划</li>
                        <li>精通主流数字营销系统及工具</li>
                        <li>用户画像及平台特性内容策划</li>
                        <li>公私域流量整合提升用户量</li>
                        <li>人人都是产品经理专栏作家</li>
                    </ul>
                </div>
                
                <div class="skill-card">
                    <h3><i class="fas fa-tasks"></i> 项目及团队管理</h3>
                    <ul class="skill-list">
                        <li>中型项目及团队管理能力</li>
                        <li>业务策略拆解及团队分工</li>
                        <li>统筹风控/产品/法务/技术/设计/客服团队</li>
                        <li>从0到1及从1到100项目经验</li>
                        <li>算法模型、AI赋能互金业务经验</li>
                        <li>银行合规改造项目实战经验</li>
                    </ul>
                </div>
            </div>
        </section>
        
        <!-- 工作经历 -->
        <section id="experience">
            <div class="section-title">
                <h2>工作经历</h2>
            </div>
            <div class="timeline">
                <!-- 苏宁银行 -->
                <div class="timeline-item">
                    <div class="timeline-period">2024.07-2025.02</div>
                    <div class="timeline-content">
                        <div class="company">
                            <div class="company-logo">
                                <i class="fas fa-university"></i>
                            </div>
                            <div class="company-info">
                                <h3>苏宁银行</h3>
                                <div class="position">普惠金融客群运营部 · 产品运营总监</div>
                            </div>
                        </div>
                        <div class="job-desc">
                            小微客群互联网信贷业务，核心KPI为信贷业务规模、用户数及活跃度（汇报对象：董事长、副行）
                        </div>
                        <div class="achievements">
                            <h4>主要成就：</h4>
                            <ul>
                                <li>搭建运营团队及用户增长体系，组建全行互联网运营项目组</li>
                                <li>搭建体系化运营管户策略，促进用户增长及转化</li>
                                <li>达成24年放款目标177.5亿元，授信新客逆势增长15%+</li>
                                <li>构建全行小微客群新媒体运营阵地，公众号综合排名行业TOP5</li>
                                <li>协同推进CRM/APP/标签体系/数据看板开发迭代</li>
                            </ul>
                        </div>
                    </div>
                </div>
                
                <!-- 蚂蚁集团 -->
                <div class="timeline-item">
                    <div class="timeline-period">2020.01-2024.05</div>
                    <div class="timeline-content">
                        <div class="company">
                            <div class="company-logo">
                                <i class="fab fa-alipay"></i>
                            </div>
                            <div class="company-info">
                                <h3>蚂蚁集团/阿里巴巴</h3>
                                <div class="position">网商银行/本地生活 · 产品运营专家</div>
                            </div>
                        </div>
                        <div class="job-desc">
                            互金产品及O2O本地电商运营，聚焦用户数及业务量增长（汇报对象：行长、业务线负责人）
                        </div>
                        <div class="achievements">
                            <h4>主要成就：</h4>
                            <ul>
                                <li>负责本地生活O2O业务运营（职级P8）</li>
                                <li>基于用户分层进行精准人群构建与营销转化</li>
                                <li>行业SAAS运营，助力商家会员及销售GMV增长</li>
                                <li>信贷产品客群线上运营，制定精细化运营策略</li>
                                <li>策划落地春耕节/丰收节、支付宝集五福等大型活动</li>
                                <li>获网商银行2022年优秀员工称号</li>
                            </ul>
                        </div>
                    </div>
                </div>
                
                <!-- 51信用卡 -->
                <div class="timeline-item">
                    <div class="timeline-period">2017.04-2019.12</div>
                    <div class="timeline-content">
                        <div class="company">
                            <div class="company-logo">
                                <i class="fas fa-credit-card"></i>
                            </div>
                            <div class="company-info">
                                <h3>51信用卡</h3>
                                <div class="position">理财业务部 · 产品运营经理</div>
                            </div>
                        </div>
                        <div class="job-desc">
                            To C个人理财类产品，核心KPI为APP用户及资金营收规模增长（汇报对象：业务线负责人）
                        </div>
                        <div class="achievements">
                            <h4>主要成就：</h4>
                            <ul>
                                <li>构建体系化的生命周期运营体系</li>
                                <li>推动产品/技术团队开发上线多项运营工具</li>
                                <li>策划"51信用卡五周年庆"活动，带来5.5亿元净充值资金</li>
                                <li>2017年超额完成年度指标，核心用户增长320%+</li>
                                <li>洽谈接入平安、百信等10多家机构理财产品</li>
                            </ul>
                        </div>
                    </div>
                </div>
                
                <!-- 东方财富 -->
                <div class="timeline-item">
                    <div class="timeline-period">2014.07-2017.04</div>
                    <div class="timeline-content">
                        <div class="company">
                            <div class="company-logo">
                                <i class="fas fa-chart-bar"></i>
                            </div>
                            <div class="company-info">
                                <h3>东方财富</h3>
                                <div class="position">个人产品部 · 用户运营/营销策划</div>
                            </div>
                        </div>
                        <div class="job-desc">
                            财经资讯及证券交易服务，核心目标为APP注册用户及证券开户数增长（汇报对象：业务线负责人）
                        </div>
                        <div class="achievements">
                            <h4>主要成就：</h4>
                            <ul>
                                <li>制订用户增长运营计划，策划项目/活动方案</li>
                                <li>策划上线30+项目/活动，如东方财富实盘炒股大赛</li>
                                <li>新开户数实现+11.93%月度增长率</li>
                                <li>输出产品需求文档182次，推动迭代发布≥100次</li>
                                <li>跟踪竞品动向，包括平安证券、同花顺等</li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </section>
        
        <!-- 项目经历 -->
        <section id="projects">
            <div class="section-title">
                <h2>项目经历</h2>
            </div>
            <div class="projects-grid">
                <div class="project-card">
                    <h3>51人品专家（用户增长）</h3>
                    <div class="project-desc">
                        通过用户MGM分享裂变机制设计，从0到1构建用户增长裂变模块
                    </div>
                    <div class="project-stats">
                        <div class="stat-item">贡献33%+平台新用户</div>
                    </div>
                </div>
                
                <div class="project-card">
                    <h3>支付宝＆KFC联名会员（精准营销）</h3>
                    <div class="project-desc">
                        通过阿里巴巴-本地生活CRM精准营销运营
                    </div>
                    <div class="project-stats">
                        <div class="stat-item">单日转化新客50000+</div>
                    </div>
                </div>
                
                <div class="project-card">
                    <h3>网商银行2021丰收节（活动运营）</h3>
                    <div class="project-desc">
                        针对性策划节点营销活动，借助支付宝流量触达客户
                    </div>
                    <div class="project-stats">
                        <div class="stat-item">转化8w+客户</div>
                        <div class="stat-item">支用超25亿元</div>
                    </div>
                </div>
                
                <div class="project-card">
                    <h3>全国县域评级模型（模型算法）</h3>
                    <div class="project-desc">
                        基于支付宝及外部区域/行业/用户数据训练模型
                    </div>
                    <div class="project-stats">
                        <div class="stat-item">业务增益120亿+</div>
                    </div>
                </div>
            </div>
        </section>
        
        <!-- 证书资质 -->
        <section id="certificates">
            <div class="section-title">
                <h2>证书资质</h2>
            </div>
            <div class="certificates">
                <div class="cert-card">
                    <h3><i class="fas fa-file-certificate"></i> 金融相关资质</h3>
                    <ul class="cert-list">
                        <li>基金从业资格</li>
                        <li>证券从业资格</li>
                        <li>银行中级从业资格</li>
                        <li>中级经济师（金融）</li>
                        <li>腾讯课堂"互金产品设计提升班"认证</li>
                    </ul>
                </div>
                
                <div class="cert-card">
                    <h3><i class="fas fa-laptop-code"></i> 互联网相关</h3>
                    <ul class="cert-list">
                        <li>PCEP国际Python程序员认证</li>
                        <li>CAIP人工智能职场应用师</li>
                        <li>C语言二级、网络编辑二级</li>
                        <li>人人都是产品经理社区-专栏作家</li>
                        <li>腾讯＆起点学院2018运营总监培训</li>
                        <li>腾讯课堂"用户增长训练营"培训认证</li>
                    </ul>
                </div>
                
                <div class="cert-card">
                    <h3><i class="fas fa-lightbulb"></i> 发明专利</h3>
                    <ul class="cert-list">
                        <li>个体属性挂载及群体属性分层大数据授信应用装置</li>
                        <li>金融风控领域（专利号CN117709963A）</li>
                    </ul>
                </div>
            </div>
        </section>
        
        <!-- 联系方式 -->
        <section id="contact" class="contact-section">
            <div class="section-title">
                <h2>联系方式</h2>
            </div>
            <div class="contact-methods">
                <div class="contact-card">
                    <div class="contact-icon">
                        <i class="fas fa-phone"></i>
                    </div>
                    <h3>电话</h3>
                    <p>18557519167</p>
                </div>
                
                <div class="contact-card">
                    <div class="contact-icon">
                        <i class="fas fa-envelope"></i>
                    </div>
                    <h3>邮箱</h3>
                    <p>shenwansan2008@163.com</p>
                </div>
                
                <div class="contact-card">
                    <div class="contact-icon">
                        <i class="fab fa-weixin"></i>
                    </div>
                    <h3>公众号</h3>
                    <p>云洲说</p>
                </div>
            </div>
        </section>
    </main>
    
    <footer>
        <div class="container">
            <p>© 2025 王伟（云洲）- 金融科技产品运营专家 | 本简历网站使用HTML5+CSS3构建</p>
        </div>
    </footer>
    
    <script>
        // 滚动动画效果
        document.addEventListener('DOMContentLoaded', function() {
            const observer = new IntersectionObserver((entries) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.style.opacity = 1;
                        entry.target.style.transform = 'translateY(0)';
                    }
                });
            }, {
                threshold: 0.1
            });
            
            // 为所有卡片添加动画
            const cards = document.querySelectorAll('.edu-item, .skill-card, .timeline-content, .project-card, .cert-card, .contact-card');
            cards.forEach(card => {
                card.style.opacity = 0;
                card.style.transform = 'translateY(20px)';
                card.style.transition = 'opacity 0.6s ease, transform 0.6s ease';
                observer.observe(card);
            });
            
            // 为标题添加动画
            const titles = document.querySelectorAll('.section-title');
            titles.forEach(title => {
                title.style.opacity = 0;
                title.style.transform = 'translateY(-20px)';
                title.style.transition = 'opacity 0.6s ease, transform 0.6s ease';
                observer.observe(title);
            });
        });
    </script>
</body>
</html>
