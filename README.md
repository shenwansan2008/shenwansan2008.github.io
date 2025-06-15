<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>王伟（云洲）- 资深金融科技运营专家</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary: #1a3a5f;
            --secondary: #2c5a8a;
            --accent: #f4a261;
            --light: #f8f9fa;
            --dark: #212529;
            --gray: #6c757d;
            --light-gray: #e9ecef;
            --success: #28a745;
            --shadow: 0 4px 12px rgba(0,0,0,0.08);
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', 'Microsoft YaHei', sans-serif;
        }
        
        body {
            background-color: #fafafa;
            color: var(--dark);
            line-height: 1.6;
            overflow-x: hidden;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* 头部样式 */
        header {
            background: linear-gradient(135deg, var(--primary) 0%, var(--secondary) 100%);
            color: white;
            padding: 30px 0;
            position: relative;
            overflow: hidden;
        }
        
        .header-content {
            display: flex;
            flex-direction: column;
            align-items: center;
            text-align: center;
            position: relative;
            z-index: 2;
        }
        
        .profile-img {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            border: 5px solid rgba(255,255,255,0.2);
            overflow: hidden;
            margin-bottom: 20px;
            box-shadow: var(--shadow);
        }
        
        .profile-img img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
        
        .header-text h1 {
            font-size: 2.2rem;
            margin-bottom: 10px;
            font-weight: 700;
        }
        
        .header-text h2 {
            font-size: 1.4rem;
            font-weight: 400;
            opacity: 0.9;
            margin-bottom: 20px;
        }
        
        .header-tags {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 10px;
            margin-top: 15px;
        }
        
        .tag {
            background: rgba(255,255,255,0.15);
            padding: 6px 15px;
            border-radius: 30px;
            font-size: 0.9rem;
            backdrop-filter: blur(4px);
        }
        
        /* 导航样式 */
        nav {
            background-color: white;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            position: sticky;
            top: 0;
            z-index: 100;
        }
        
        .nav-container {
            display: flex;
            justify-content: center;
        }
        
        .nav-links {
            display: flex;
            list-style: none;
            overflow-x: auto;
            padding: 0 15px;
            -ms-overflow-style: none;
            scrollbar-width: none;
        }
        
        .nav-links::-webkit-scrollbar {
            display: none;
        }
        
        .nav-links li {
            flex-shrink: 0;
        }
        
        .nav-links a {
            display: block;
            padding: 18px 20px;
            text-decoration: none;
            color: var(--gray);
            font-weight: 500;
            transition: all 0.3s;
            position: relative;
        }
        
        .nav-links a:hover,
        .nav-links a.active {
            color: var(--primary);
        }
        
        .nav-links a.active:after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 20%;
            width: 60%;
            height: 3px;
            background: var(--accent);
            border-radius: 3px;
        }
        
        /* 主要内容区域 */
        section {
            padding: 60px 0;
            background: white;
            margin-bottom: 20px;
            border-radius: 10px;
            box-shadow: var(--shadow);
        }
        
        .section-header {
            text-align: center;
            margin-bottom: 40px;
            position: relative;
        }
        
        .section-header h2 {
            font-size: 2rem;
            color: var(--primary);
            margin-bottom: 15px;
            display: inline-block;
            position: relative;
        }
        
        .section-header h2:after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 70px;
            height: 4px;
            background: var(--accent);
            border-radius: 2px;
        }
        
        .section-header p {
            color: var(--gray);
            max-width: 700px;
            margin: 20px auto 0;
        }
        
        /* 教育背景 */
        .education-container {
            display: grid;
            grid-template-columns: 1fr;
            gap: 30px;
            max-width: 800px;
            margin: 0 auto;
        }
        
        .education-item {
            display: flex;
            background: var(--light);
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 3px 10px rgba(0,0,0,0.05);
            transition: transform 0.3s;
        }
        
        .education-item:hover {
            transform: translateY(-5px);
        }
        
        .edu-logo {
            flex: 0 0 90px;
            background: var(--primary);
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 2.5rem;
        }
        
        .edu-content {
            padding: 25px;
            flex: 1;
        }
        
        .edu-content h3 {
            font-size: 1.4rem;
            margin-bottom: 8px;
            color: var(--primary);
        }
        
        .edu-meta {
            display: flex;
            flex-wrap: wrap;
            gap: 15px;
            margin: 10px 0 15px;
            color: var(--gray);
            font-size: 0.95rem;
        }
        
        .edu-meta span {
            display: flex;
            align-items: center;
        }
        
        .edu-meta i {
            margin-right: 6px;
            color: var(--accent);
        }
        
        .edu-achievements {
            margin-top: 15px;
            padding-top: 15px;
            border-top: 1px solid var(--light-gray);
        }
        
        .edu-achievements ul {
            list-style: none;
        }
        
        .edu-achievements li {
            margin-bottom: 8px;
            display: flex;
            align-items: flex-start;
        }
        
        .edu-achievements li:before {
            content: '✓';
            color: var(--success);
            font-weight: bold;
            margin-right: 10px;
        }
        
        /* 技能特长 */
        .skills-container {
            display: grid;
            grid-template-columns: 1fr;
            gap: 30px;
        }
        
        .skill-category {
            background: var(--light);
            border-radius: 10px;
            padding: 30px;
            box-shadow: 0 3px 15px rgba(0,0,0,0.05);
            transition: all 0.3s;
        }
        
        .skill-category:hover {
            transform: translateY(-5px);
            box-shadow: 0 5px 20px rgba(0,0,0,0.1);
        }
        
        .skill-header {
            display: flex;
            align-items: center;
            margin-bottom: 20px;
        }
        
        .skill-icon {
            width: 60px;
            height: 60px;
            background: var(--primary);
            border-radius: 12px;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-right: 20px;
            color: white;
            font-size: 1.8rem;
        }
        
        .skill-title {
            font-size: 1.5rem;
            color: var(--primary);
        }
        
        .skill-items {
            list-style: none;
        }
        
        .skill-items li {
            margin-bottom: 15px;
            padding-bottom: 15px;
            border-bottom: 1px dashed var(--light-gray);
        }
        
        .skill-items li:last-child {
            margin-bottom: 0;
            padding-bottom: 0;
            border-bottom: none;
        }
        
        .skill-items li strong {
            display: block;
            margin-bottom: 5px;
            color: var(--secondary);
        }
        
        /* 工作经历 */
        .timeline {
            position: relative;
            max-width: 900px;
            margin: 0 auto;
        }
        
        .timeline:before {
            content: '';
            position: absolute;
            top: 0;
            bottom: 0;
            width: 4px;
            background: var(--light-gray);
            left: 50%;
            margin-left: -2px;
        }
        
        .timeline-item {
            position: relative;
            margin-bottom: 50px;
            display: flex;
        }
        
        .timeline-item:nth-child(odd) {
            justify-content: flex-start;
            padding-right: calc(50% + 30px);
        }
        
        .timeline-item:nth-child(even) {
            justify-content: flex-end;
            padding-left: calc(50% + 30px);
        }
        
        .timeline-content {
            background: white;
            border-radius: 10px;
            padding: 30px;
            box-shadow: var(--shadow);
            width: 100%;
            position: relative;
            border: 1px solid var(--light-gray);
        }
        
        .timeline-content:before {
            content: '';
            position: absolute;
            top: 30px;
            width: 20px;
            height: 20px;
            background: white;
            border: 4px solid var(--accent);
            border-radius: 50%;
        }
        
        .timeline-item:nth-child(odd) .timeline-content:before {
            right: -40px;
        }
        
        .timeline-item:nth-child(even) .timeline-content:before {
            left: -40px;
        }
        
        .timeline-header {
            display: flex;
            align-items: center;
            margin-bottom: 15px;
        }
        
        .company-logo {
            width: 50px;
            height: 50px;
            background: var(--light);
            border-radius: 10px;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-right: 15px;
            color: var(--primary);
            font-size: 1.5rem;
            flex-shrink: 0;
        }
        
        .company-info {
            flex: 1;
        }
        
        .company-info h3 {
            font-size: 1.4rem;
            color: var(--primary);
            margin-bottom: 5px;
        }
        
        .company-meta {
            color: var(--gray);
            font-size: 0.95rem;
        }
        
        .timeline-content ul {
            padding-left: 20px;
            margin-top: 15px;
        }
        
        .timeline-content ul li {
            margin-bottom: 12px;
            position: relative;
        }
        
        .timeline-content ul li:before {
            content: '•';
            color: var(--accent);
            font-weight: bold;
            position: absolute;
            left: -20px;
        }
        
        .timeline-highlight {
            background: rgba(244, 162, 97, 0.1);
            border-left: 3px solid var(--accent);
            padding: 15px;
            margin-top: 15px;
            border-radius: 0 8px 8px 0;
            font-size: 0.95rem;
        }
        
        /* 项目经历 */
        .projects-container {
            display: grid;
            grid-template-columns: 1fr;
            gap: 30px;
        }
        
        .project-card {
            background: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: var(--shadow);
            border: 1px solid var(--light-gray);
            transition: all 0.3s;
        }
        
        .project-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0,0,0,0.1);
        }
        
        .project-header {
            background: var(--primary);
            color: white;
            padding: 20px;
        }
        
        .project-header h3 {
            font-size: 1.4rem;
            margin-bottom: 5px;
        }
        
        .project-category {
            opacity: 0.8;
            font-size: 0.95rem;
        }
        
        .project-content {
            padding: 25px;
        }
        
        .project-stats {
            display: flex;
            justify-content: space-around;
            text-align: center;
            margin: 20px 0;
            padding: 15px 0;
            background: var(--light);
            border-radius: 8px;
        }
        
        .stat-item h4 {
            font-size: 1.8rem;
            color: var(--accent);
            margin-bottom: 5px;
        }
        
        .stat-item p {
            font-size: 0.9rem;
            color: var(--gray);
        }
        
        .project-desc {
            line-height: 1.7;
            color: var(--dark);
        }
        
        /* 证书资质 */
        .certificates {
            display: grid;
            grid-template-columns: 1fr;
            gap: 20px;
        }
        
        .cert-category {
            margin-bottom: 30px;
        }
        
        .cert-category h3 {
            font-size: 1.4rem;
            color: var(--primary);
            margin-bottom: 20px;
            padding-bottom: 10px;
            border-bottom: 2px solid var(--light-gray);
        }
        
        .cert-list {
            display: grid;
            grid-template-columns: 1fr;
            gap: 15px;
        }
        
        .cert-item {
            background: var(--light);
            padding: 15px 20px;
            border-radius: 8px;
            display: flex;
            align-items: center;
            box-shadow: 0 3px 8px rgba(0,0,0,0.05);
        }
        
        .cert-icon {
            width: 40px;
            height: 40px;
            background: var(--primary);
            border-radius: 8px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            margin-right: 15px;
            flex-shrink: 0;
        }
        
        .cert-name {
            flex: 1;
        }
        
        .cert-badge {
            background: var(--accent);
            color: white;
            padding: 3px 10px;
            border-radius: 30px;
            font-size: 0.85rem;
            margin-left: 10px;
        }
        
        /* 联系方式 */
        .contact-container {
            display: grid;
            grid-template-columns: 1fr;
            gap: 30px;
        }
        
        .contact-info {
            background: linear-gradient(135deg, var(--primary) 0%, var(--secondary) 100%);
            border-radius: 10px;
            padding: 40px;
            color: white;
            box-shadow: var(--shadow);
        }
        
        .contact-info h3 {
            font-size: 1.6rem;
            margin-bottom: 25px;
            text-align: center;
        }
        
        .contact-item {
            display: flex;
            align-items: center;
            margin-bottom: 20px;
        }
        
        .contact-icon {
            width: 50px;
            height: 50px;
            background: rgba(255,255,255,0.15);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-right: 20px;
            font-size: 1.3rem;
            flex-shrink: 0;
        }
        
        .contact-details {
            flex: 1;
        }
        
        .contact-details h4 {
            font-size: 1.1rem;
            margin-bottom: 5px;
        }
        
        .contact-details a {
            color: white;
            text-decoration: none;
            transition: opacity 0.3s;
        }
        
        .contact-details a:hover {
            opacity: 0.8;
            text-decoration: underline;
        }
        
        .qr-code {
            text-align: center;
            margin-top: 20px;
            padding-top: 20px;
            border-top: 1px solid rgba(255,255,255,0.2);
        }
        
        .qr-code img {
            width: 150px;
            height: 150px;
            margin-bottom: 10px;
        }
        
        .qr-code p {
            font-size: 0.9rem;
            opacity: 0.9;
        }
        
        footer {
            background: var(--dark);
            color: white;
            text-align: center;
            padding: 30px 0;
            margin-top: 50px;
        }
        
        /* 响应式设计 */
        @media (min-width: 576px) {
            .skills-container,
            .projects-container {
                grid-template-columns: repeat(2, 1fr);
            }
            
            .cert-list {
                grid-template-columns: repeat(2, 1fr);
            }
        }
        
        @media (min-width: 768px) {
            .header-content {
                flex-direction: row;
                text-align: left;
                align-items: center;
            }
            
            .profile-img {
                margin-right: 40px;
                margin-bottom: 0;
            }
            
            .header-text h1 {
                font-size: 2.5rem;
            }
            
            .header-text h2 {
                font-size: 1.6rem;
            }
            
            .section-header h2 {
                font-size: 2.2rem;
            }
            
            .education-container {
                grid-template-columns: 1fr;
            }
            
            .contact-container {
                grid-template-columns: 1fr 1fr;
            }
        }
        
        @media (min-width: 992px) {
            .skills-container {
                grid-template-columns: repeat(2, 1fr);
            }
            
            .projects-container {
                grid-template-columns: repeat(3, 1fr);
            }
            
            .cert-list {
                grid-template-columns: repeat(3, 1fr);
            }
        }
        
        @media (max-width: 767px) {
            .timeline:before {
                left: 30px;
            }
            
            .timeline-item {
                padding-left: 70px !important;
                padding-right: 0 !important;
            }
            
            .timeline-item:nth-child(odd),
            .timeline-item:nth-child(even) {
                justify-content: flex-start;
            }
            
            .timeline-content:before {
                left: -40px !important;
            }
        }
        
        /* 微信浏览器特别优化 */
        @media (-webkit-min-device-pixel-ratio:0) and (max-device-width: 1024px) {
            body {
                -webkit-text-size-adjust: 100%;
            }
            
            .nav-links {
                padding-bottom: 5px;
            }
            
            .nav-links a {
                padding: 15px 16px;
                font-size: 0.95rem;
            }
        }
    </style>
</head>
<body>
    <!-- 头部区域 -->
    <header>
        <div class="container">
            <div class="header-content">
                <div class="profile-img">
                    <img src="https://s21.ax1x.com/2025/06/15/pVAqWF0.jpg" alt="王伟">
                </div>
                <div class="header-text">
                    <h1>王伟（云洲）</h1>
                    <h2>金融科技/互联网产品运营总监</h2>
                    <div class="header-tags">
                        <div class="tag">前一线大厂产品运营专家</div>
                        <div class="tag">10年+金融科技/电商经验</div>
                        <div class="tag">体系化产品运营管理方法论</div>
                    </div>
                </div>
            </div>
        </div>
    </header>

    <!-- 导航区域 -->
    <nav>
        <div class="nav-container">
            <ul class="nav-links">
                <li><a href="#education" class="active">教育背景</a></li>
                <li><a href="#skills">技能特长</a></li>
                <li><a href="#experience">工作经历</a></li>
                <li><a href="#projects">项目经历</a></li>
                <li><a href="#certificates">证书资质</a></li>
                <li><a href="#contact">联系方式</a></li>
            </ul>
        </div>
    </nav>

    <!-- 主要内容区域 -->
    <main class="container">
        <!-- 教育背景 -->
        <section id="education">
            <div class="section-header">
                <h2>教育背景</h2>
                <p>扎实的教育背景为职业发展奠定坚实基础</p>
            </div>
            <div class="education-container">
                <div class="education-item">
                    <div class="edu-logo">
                        <i class="fas fa-university"></i>
                    </div>
                    <div class="edu-content">
                        <h3>南京大学（985）</h3>
                        <div class="edu-meta">
                            <span><i class="fas fa-graduation-cap"></i> 信息管理学院-数字出版专业</span>
                            <span><i class="fas fa-calendar-alt"></i> 2011.09-2014.06</span>
                        </div>
                        <p>班长/研会主席，2013国家奖学金，优秀毕业生</p>
                        <div class="edu-achievements">
                            <ul>
                                <li>担任研究生会主席，组织多场学术活动</li>
                                <li>获得国家奖学金（全国研究生前2%）</li>
                                <li>优秀毕业生荣誉获得者</li>
                            </ul>
                        </div>
                    </div>
                </div>
                
                <div class="education-item">
                    <div class="edu-logo">
                        <i class="fas fa-book"></i>
                    </div>
                    <div class="edu-content">
                        <h3>安徽大学（211）</h3>
                        <div class="edu-meta">
                            <span><i class="fas fa-graduation-cap"></i> 汉语言文学（辅修工商管理）</span>
                            <span><i class="fas fa-calendar-alt"></i> 2003.10-2007.06</span>
                        </div>
                        <p>学生会部长，安大优秀毕业生</p>
                        <div class="edu-achievements">
                            <ul>
                                <li>担任学生会部长，领导团队组织校园活动</li>
                                <li>辅修工商管理，拓展了商业视野</li>
                                <li>优秀毕业生荣誉获得者</li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- 技能特长 -->
        <section id="skills">
            <div class="section-header">
                <h2>技能特长</h2>
                <p>丰富的运营管理经验与专业技能</p>
            </div>
            <div class="skills-container">
                <div class="skill-category">
                    <div class="skill-header">
                        <div class="skill-icon">
                            <i class="fas fa-users"></i>
                        </div>
                        <h3 class="skill-title">用户运营</h3>
                    </div>
                    <ul class="skill-items">
                        <li>
                            <strong>亿级用户运营</strong>
                            拥有亿级用户平台运营经验，熟悉用户生命周期管理
                        </li>
                        <li>
                            <strong>分层运营策略</strong>
                            擅长基于用户画像进行精细化分层运营
                        </li>
                        <li>
                            <strong>增长黑客</strong>
                            从0到1搭建用户增长体系，实现平台用户年增300%+
                        </li>
                        <li>
                            <strong>活动策划</strong>
                            策划执行大型营销活动，单次活动促成25亿+信贷支用
                        </li>
                    </ul>
                </div>
                
                <div class="skill-category">
                    <div class="skill-header">
                        <div class="skill-icon">
                            <i class="fas fa-mobile-alt"></i>
                        </div>
                        <h3 class="skill-title">产品运营</h3>
                    </div>
                    <ul class="skill-items">
                        <li>
                            <strong>产品迭代优化</strong>
                            擅长APP运营、活动运营、流量精细化运营等
                        </li>
                        <li>
                            <strong>数据分析能力</strong>
                            熟练使用Python、SQL、Excel等BI工具进行数据分析
                        </li>
                        <li>
                            <strong>工具应用</strong>
                            精通Axure、XMind、ProcessOn等产品设计工具
                        </li>
                        <li>
                            <strong>用户洞察</strong>
                            结合用户反馈、指标监测、AB测试推动产品优化
                        </li>
                    </ul>
                </div>
                
                <div class="skill-category">
                    <div class="skill-header">
                        <div class="skill-icon">
                            <i class="fas fa-chart-line"></i>
                        </div>
                        <h3 class="skill-title">内容/流量运营</h3>
                    </div>
                    <ul class="skill-items">
                        <li>
                            <strong>流量精细化运营</strong>
                            精通主流数字营销系统及工具，优化渠道投放
                        </li>
                        <li>
                            <strong>新媒体运营</strong>
                            从0到1构建新媒体运营阵地，公众号排名行业TOP5
                        </li>
                        <li>
                            <strong>内容策划</strong>
                            结合用户画像及平台特性策划优质内容
                        </li>
                        <li>
                            <strong>公私域流量整合</strong>
                            综合运用公私域流量提升用户量及品牌影响力
                        </li>
                    </ul>
                </div>
                
                <div class="skill-category">
                    <div class="skill-header">
                        <div class="skill-icon">
                            <i class="fas fa-tasks"></i>
                        </div>
                        <h3 class="skill-title">项目及团队管理</h3>
                    </div>
                    <ul class="skill-items">
                        <li>
                            <strong>跨部门协作</strong>
                            统筹风控/产品/法务/技术/设计/客服团队推进项目
                        </li>
                        <li>
                            <strong>团队建设</strong>
                            搭建运营团队及用户增长体系，制定业务指标
                        </li>
                        <li>
                            <strong>项目管理</strong>
                            丰富从0到1及从1到100的项目管理经验
                        </li>
                        <li>
                            <strong>风险合规</strong>
                            熟悉金融行业政策法规，风险合规意识强
                        </li>
                    </ul>
                </div>
            </div>
        </section>

        <!-- 工作经历 -->
        <section id="experience">
            <div class="section-header">
                <h2>工作经历</h2>
                <p>丰富的金融科技与互联网运营管理经验</p>
            </div>
            <div class="timeline">
                <!-- 苏宁银行 -->
                <div class="timeline-item">
                    <div class="timeline-content">
                        <div class="timeline-header">
                            <div class="company-logo">
                                <i class="fas fa-building"></i>
                            </div>
                            <div class="company-info">
                                <h3>苏宁银行</h3>
                                <div class="company-meta">
                                    <span>普惠金融客群运营部 - 产品运营总监</span>
                                    <span>2024年7月 - 2025年2月</span>
                                </div>
                            </div>
                        </div>
                        <p>负责小微客群互联网信贷业务，核心KPI为信贷业务规模、用户数及活跃度</p>
                        <ul>
                            <li>搭建运营团队及用户增长体系，制订团队业务指标并统筹业务策略落地</li>
                            <li>跨部门组建全行层面的互联网运营项目组，提升全行互联网运营水平</li>
                            <li>搭建体系化的运营管户策略，促进用户增长及转化，达成24年放款目标177.5亿元</li>
                            <li>以公众号/视频号为抓手，从0到1构建全行小微客群新媒体运营阵地</li>
                        </ul>
                        <div class="timeline-highlight">
                            <strong>突出业绩：</strong>授信新客逆势增长15%+，不良率仅1.32%；公众号综合排名跻身行业TOP5，粉丝数实现200%+增长
                        </div>
                    </div>
                </div>
                
                <!-- 蚂蚁集团 -->
                <div class="timeline-item">
                    <div class="timeline-content">
                        <div class="timeline-header">
                            <div class="company-logo">
                                <i class="fab fa-alipay"></i>
                            </div>
                            <div class="company-info">
                                <h3>蚂蚁集团/阿里巴巴</h3>
                                <div class="company-meta">
                                    <span>网商银行/本地生活 - 产品运营专家</span>
                                    <span>2020年1月 - 2024年5月</span>
                                </div>
                            </div>
                        </div>
                        <p>互金产品及O2O本地电商运营，聚焦用户数及业务量增长</p>
                        <ul>
                            <li>负责本地生活O2O业务运营，基于用户分层进行精准营销转化</li>
                            <li>行业SAAS运营，链接B端商家与C端用户，助力商家会员及销售GMV增长</li>
                            <li>负责信贷产品客群线上运营，统筹制定客群精细化运营策略</li>
                            <li>独立策划各类型业务营销活动，综合运用公私域流量触达客户</li>
                        </ul>
                        <div class="timeline-highlight">
                            <strong>突出业绩：</strong>获网商银行2022年优秀员工称号；网商银行2021丰收节单场活动促成8w+客户信贷支用25亿+
                        </div>
                    </div>
                </div>
                
                <!-- 51信用卡 -->
                <div class="timeline-item">
                    <div class="timeline-content">
                        <div class="timeline-header">
                            <div class="company-logo">
                                <i class="fas fa-credit-card"></i>
                            </div>
                            <div class="company-info">
                                <h3>51信用卡</h3>
                                <div class="company-meta">
                                    <span>理财业务部 - 产品运营经理</span>
                                    <span>2017.04 - 2019.12</span>
                                </div>
                            </div>
                        </div>
                        <p>To C个人理财类产品，核心KPI为APP用户及资金营收规模增长</p>
                        <ul>
                            <li>构建体系化的生命周期运营体系，包括新手链路、用户成长、老带新裂变等</li>
                            <li>推动开发上线多项运营工具，构建数据报表＆业务增长模型</li>
                            <li>构建活动运营矩阵，策划执行"51信用卡五周年庆"等大型活动</li>
                            <li>开展机构异业合作，接入平安、百信等10多家机构理财产品</li>
                        </ul>
                        <div class="timeline-highlight">
                            <strong>突出业绩：</strong>2017年超额完成年度指标，核心用户增长320%+，全年累计净募资77.6亿
                        </div>
                    </div>
                </div>
                
                <!-- 东方财富 -->
                <div class="timeline-item">
                    <div class="timeline-content">
                        <div class="timeline-header">
                            <div class="company-logo">
                                <i class="fas fa-chart-bar"></i>
                            </div>
                            <div class="company-info">
                                <h3>东方财富</h3>
                                <div class="company-meta">
                                    <span>个人产品部 - 用户运营/营销策划</span>
                                    <span>2014.07 - 2017.04</span>
                                </div>
                            </div>
                        </div>
                        <p>财经资讯及证券交易服务，核心目标为APP注册用户及证券开户数增长</p>
                        <ul>
                            <li>制订用户增长运营计划，策划项目/活动方案促进用户增长</li>
                            <li>策划上线30+项目/活动，如东方财富实盘炒股大赛</li>
                            <li>持续优化产品及项目流程，提升用户体验</li>
                            <li>关注行业动态，跟踪竞品动向策划选题</li>
                        </ul>
                        <div class="timeline-highlight">
                            <strong>突出业绩：</strong>促成新开户数实现+11.93%月度增长率；累计输出产品需求文档182次
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- 项目经历 -->
        <section id="projects">
            <div class="section-header">
                <h2>项目经历</h2>
                <p>成功主导并参与多个重要项目</p>
            </div>
            <div class="projects-container">
                <div class="project-card">
                    <div class="project-header">
                        <h3>网商银行2021丰收节</h3>
                        <div class="project-category">活动运营</div>
                    </div>
                    <div class="project-content">
                        <div class="project-stats">
                            <div class="stat-item">
                                <h4>25亿+</h4>
                                <p>信贷支用金额</p>
                            </div>
                            <div class="stat-item">
                                <h4>8万+</h4>
                                <p>转化客户</p>
                            </div>
                        </div>
                        <div class="project-desc">
                            <p>针对性策划节点营销活动，借助支付宝流量触达客户，通过免息贷款/利率优惠券/积分/支付宝红包等权益工具促成客户转化。</p>
                            <p><strong>创新点：</strong>综合运用支付宝app公域、网商银行私域及外部渠道流量触达客户。</p>
                        </div>
                    </div>
                </div>
                
                <div class="project-card">
                    <div class="project-header">
                        <h3>支付宝＆KFC联名会员</h3>
                        <div class="project-category">精准营销</div>
                    </div>
                    <div class="project-content">
                        <div class="project-stats">
                            <div class="stat-item">
                                <h4>50,000+</h4>
                                <p>单日新客转化</p>
                            </div>
                            <div class="stat-item">
                                <h4>行业TOP</h4>
                                <p>头部企业合作</p>
                            </div>
                        </div>
                        <div class="project-desc">
                            <p>通过阿里巴巴-本地生活CRM精准营销运营，链接B端商家与C端用户，助力商家会员及销售GMV增长。</p>
                            <p><strong>创新点：</strong>基于支付宝/饿了么平台流量及产品能力，以CRM系统会员运营为核心能力。</p>
                        </div>
                    </div>
                </div>
                
                <div class="project-card">
                    <div class="project-header">
                        <h3>51人品专家</h3>
                        <div class="project-category">用户增长</div>
                    </div>
                    <div class="project-content">
                        <div class="project-stats">
                            <div class="stat-item">
                                <h4>33%+</h4>
                                <p>平台新用户贡献</p>
                            </div>
                            <div class="stat-item">
                                <h4>裂变机制</h4>
                                <p>创新设计</p>
                            </div>
                        </div>
                        <div class="project-desc">
                            <p>通过用户MGM分享裂变机制设计，从0到1构建用户增长裂变模块，围绕新手链路、用户成长、老带新裂变等场景构建体系。</p>
                            <p><strong>创新点：</strong>结合红包裂变等拉新模块，聚焦头部客户的"VIP会员体系"。</p>
                        </div>
                    </div>
                </div>
                
                <div class="project-card">
                    <div class="project-header">
                        <h3>全国县域评级模型</h3>
                        <div class="project-category">模型算法</div>
                    </div>
                    <div class="project-content">
                        <div class="project-stats">
                            <div class="stat-item">
                                <h4>120亿+</h4>
                                <p>业务增益</p>
                            </div>
                            <div class="stat-item">
                                <h4>大数据</h4>
                                <p>授信应用</p>
                            </div>
                        </div>
                        <div class="project-desc">
                            <p>基于支付宝及外部区域/行业/用户数据训练模型，实现全国县域中宏观评级，为信贷决策提供数据支持。</p>
                            <p><strong>创新点：</strong>该项目获得发明专利"个体属性挂载及群体属性分层大数据授信应用装置"。</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- 证书资质 -->
        <section id="certificates">
            <div class="section-header">
                <h2>证书资质</h2>
                <p>专业认证与行业资质</p>
            </div>
            <div class="certificates">
                <div class="cert-category">
                    <h3>金融相关资质</h3>
                    <div class="cert-list">
                        <div class="cert-item">
                            <div class="cert-icon">
                                <i class="fas fa-file-invoice-dollar"></i>
                            </div>
                            <div class="cert-name">基金从业资格</div>
                        </div>
                        <div class="cert-item">
                            <div class="cert-icon">
                                <i class="fas fa-chart-line"></i>
                            </div>
                            <div class="cert-name">证券从业资格</div>
                        </div>
                        <div class="cert-item">
                            <div class="cert-icon">
                                <i class="fas fa-university"></i>
                            </div>
                            <div class="cert-name">银行中级从业资格</div>
                        </div>
                        <div class="cert-item">
                            <div class="cert-icon">
                                <i class="fas fa-coins"></i>
                            </div>
                            <div class="cert-name">中级经济师（金融）</div>
                        </div>
                        <div class="cert-item">
                            <div class="cert-icon">
                                <i class="fab fa-weixin"></i>
                            </div>
                            <div class="cert-name">腾讯课堂"互金产品设计提升班"认证</div>
                        </div>
                    </div>
                </div>
                
                <div class="cert-category">
                    <h3>互联网相关</h3>
                    <div class="cert-list">
                        <div class="cert-item">
                            <div class="cert-icon">
                                <i class="fab fa-python"></i>
                            </div>
                            <div class="cert-name">PCEP国际Python程序员认证</div>
                        </div>
                        <div class="cert-item">
                            <div class="cert-icon">
                                <i class="fas fa-robot"></i>
                            </div>
                            <div class="cert-name">CAIP人工智能职场应用师</div>
                        </div>
                        <div class="cert-item">
                            <div class="cert-icon">
                                <i class="fas fa-code"></i>
                            </div>
                            <div class="cert-name">C语言二级</div>
                        </div>
                        <div class="cert-item">
                            <div class="cert-icon">
                                <i class="fas fa-edit"></i>
                            </div>
                            <div class="cert-name">网络编辑二级</div>
                        </div>
                        <div class="cert-item">
                            <div class="cert-icon">
                                <i class="fas fa-pen-fancy"></i>
                            </div>
                            <div class="cert-name">人人都是产品经理社区-专栏作家</div>
                        </div>
                    </div>
                </div>
                
                <div class="cert-category">
                    <h3>专利与培训</h3>
                    <div class="cert-list">
                        <div class="cert-item">
                            <div class="cert-icon">
                                <i class="fas fa-gem"></i>
                            </div>
                            <div class="cert-name">
                                专利：个体属性挂载及群体属性分层大数据授信应用装置
                                <span class="cert-badge">发明专利</span>
                            </div>
                        </div>
                        <div class="cert-item">
                            <div class="cert-icon">
                                <i class="fas fa-graduation-cap"></i>
                            </div>
                            <div class="cert-name">腾讯＆起点学院2018运营总监培训</div>
                        </div>
                        <div class="cert-item">
                            <div class="cert-icon">
                                <i class="fas fa-users"></i>
                            </div>
                            <div class="cert-name">腾讯课堂"用户增长训练营"培训认证</div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- 联系方式 -->
        <section id="contact">
            <div class="section-header">
                <h2>联系方式</h2>
                <p>期待与您建立联系</p>
            </div>
            <div class="contact-container">
                <div class="contact-info">
                    <h3>联系信息</h3>
                    <div class="contact-item">
                        <div class="contact-icon">
                            <i class="fas fa-phone-alt"></i>
                        </div>
                        <div class="contact-details">
                            <h4>电话</h4>
                            <a href="tel:18557519167">18557519167</a>
                        </div>
                    </div>
                    <div class="contact-item">
                        <div class="contact-icon">
                            <i class="fas fa-envelope"></i>
                        </div>
                        <div class="contact-details">
                            <h4>邮箱</h4>
                            <a href="mailto:shenwansan2008@163.com">shenwansan2008@163.com</a>
                        </div>
                    </div>
                    <div class="contact-item">
                        <div class="contact-icon">
                            <i class="fab fa-weixin"></i>
                        </div>
                        <div class="contact-details">
                            <h4>公众号</h4>
                            <span>云洲说yunzhoushuo</span>
                        </div>
                    </div>
                    <div class="contact-item">
                        <div class="contact-icon">
                            <i class="fas fa-map-marker-alt"></i>
                        </div>
                        <div class="contact-details">
                            <h4>所在地</h4>
                            <span>浙江省杭州市</span>
                        </div>
                    </div>
                    <div class="qr-code">
                        <img src="https://s21.ax1x.com/2025/06/15/pVAvMvT.png" alt="个人微信二维码">
                        <p>扫码添加微信</p>
                    </div>
                </div>
                
                <div class="contact-form">
                    <div style="background:#f8f9fa;padding:40px;border-radius:10px;height:100%;">
                        <h3 style="text-align:center;margin-bottom:30px;color:var(--primary);">立即联系</h3>
                        <p style="text-align:center;margin-bottom:30px;">如果您有任何合作意向或职位机会，欢迎随时与我联系。我期待与优秀的团队共同创造价值。</p>
                        <div style="text-align:center;margin-top:40px;">
                            <a href="mailto:shenwansan2008@163.com" style="display:inline-block;background:var(--accent);color:white;padding:15px 40px;border-radius:30px;text-decoration:none;font-weight:bold;transition:all 0.3s;">发送邮件</a>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </main>

    <!-- 页脚 -->
    <footer>
        <div class="container">
            <p>© 2025 王伟（云洲）- 金融科技/互联网产品运营专家</p>
            <p>本网站使用HTML5+CSS3开发，适配移动端与PC端</p>
        </div>
    </footer>

    <script>
        // 导航滚动效果
        document.addEventListener('DOMContentLoaded', function() {
            const navLinks = document.querySelectorAll('.nav-links a');
            
            navLinks.forEach(link => {
                link.addEventListener('click', function(e) {
                    e.preventDefault();
                    
                    // 移除所有active类
                    navLinks.forEach(l => l.classList.remove('active'));
                    
                    // 添加当前active类
                    this.classList.add('active');
                    
                    // 滚动到目标区域
                    const targetId = this.getAttribute('href');
                    const targetSection = document.querySelector(targetId);
                    const headerOffset = 100;
                    const elementPosition = targetSection.getBoundingClientRect().top;
                    const offsetPosition = elementPosition + window.pageYOffset - headerOffset;
                    
                    window.scrollTo({
                        top: offsetPosition,
                        behavior: 'smooth'
                    });
                });
            });
            
            // 滚动时高亮当前区域
            window.addEventListener('scroll', function() {
                const sections = document.querySelectorAll('section');
                let current = '';
                
                sections.forEach(section => {
                    const sectionTop = section.offsetTop;
                    const sectionHeight = section.clientHeight;
                    
                    if (pageYOffset >= (sectionTop - 150)) {
                        current = section.getAttribute('id');
                    }
                });
                
                navLinks.forEach(link => {
                    link.classList.remove('active');
                    if (link.getAttribute('href') === '#' + current) {
                        link.classList.add('active');
                    }
                });
            });
            
            // 移动端导航优化
            if (window.innerWidth < 768) {
                const nav = document.querySelector('.nav-links');
                let startX = 0;
                let scrollLeft = 0;
                
                nav.addEventListener('touchstart', function(e) {
                    startX = e.touches[0].pageX;
                    scrollLeft = nav.scrollLeft;
                });
                
                nav.addEventListener('touchmove', function(e) {
                    e.preventDefault();
                    const x = e.touches[0].pageX;
                    const walk = (x - startX) * 2;
                    nav.scrollLeft = scrollLeft - walk;
                });
            }
        });
    </script>
</body>
</html>
