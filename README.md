<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>鸣金虹流派PVP完全攻略 | 燕云十六声 - 2026.12</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        /* 基础重置与水墨风格 - PDF优化版 */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Microsoft YaHei', 'STKaiti', serif;
            background: white !important;
            color: #333;
            line-height: 1.6;
            padding: 0;
            margin: 0;
            -webkit-print-color-adjust: exact;
            print-color-adjust: exact;
        }
        
        /* PDF专用页面设置 */
        @page {
            size: A4;
            margin: 1.5cm;
        }
        
        @page :first {
            margin-top: 2cm;
        }
        
        /* 主内容容器 */
        .main-container {
            width: 100%;
            max-width: 21cm;
            margin: 0 auto;
            padding: 0.5cm;
            background: white;
            box-sizing: border-box;
        }
        
        /* 标题与页眉 */
        .header-section {
            text-align: center;
            margin-bottom: 1.2cm;
            padding: 0.8cm;
            background: linear-gradient(135deg, #fff 0%, #f8f3ea 100%);
            border-radius: 0.3cm;
            border: 0.05cm solid rgba(139, 69, 19, 0.1);
            position: relative;
            overflow: hidden;
            page-break-after: avoid;
        }
        
        .header-section::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 0.1cm;
            background: linear-gradient(90deg, #8B4513 0%, #D2B48C 50%, #8B4513 100%);
        }
        
        .header-section h1 {
            font-size: 1.8rem;
            color: #5D2E1F;
            margin-bottom: 0.3cm;
            letter-spacing: 0.05cm;
            position: relative;
            display: inline-block;
            padding-bottom: 0.4cm;
        }
        
        .header-section h1::after {
            content: "";
            position: absolute;
            bottom: 0;
            left: 25%;
            right: 25%;
            height: 0.08cm;
            background: linear-gradient(90deg, transparent 0%, #8B4513 50%, transparent 100%);
        }
        
        .header-section .subtitle {
            font-size: 0.9rem;
            color: #8B4513;
            font-style: italic;
            margin-bottom: 0.5cm;
            opacity: 0.9;
        }
        
        .header-tags {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 0.3cm;
            margin-top: 0.5cm;
        }
        
        /* 卡片容器 */
        .card-container {
            width: 100%;
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 0.8cm;
            margin-bottom: 1cm;
        }
        
        /* 卡片样式 */
        .card {
            background: linear-gradient(to bottom, #fff 0%, #fcf9f5 100%);
            border-radius: 0.3cm;
            box-shadow: 0 0.2cm 0.5cm rgba(139, 69, 19, 0.08);
            padding: 0.8cm;
            border: 0.03cm solid rgba(139, 69, 19, 0.1);
            position: relative;
            overflow: hidden;
            width: 100%;
            page-break-inside: avoid;
        }
        
        .card::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            width: 0.2cm;
            height: 100%;
            background: linear-gradient(to bottom, #8B4513 0%, #D2B48C 100%);
        }
        
        .card-header {
            display: flex;
            align-items: center;
            margin-bottom: 0.6cm;
            padding-bottom: 0.5cm;
            border-bottom: 0.03cm solid rgba(139, 69, 19, 0.1);
        }
        
        .card-icon {
            font-size: 1.2rem;
            color: #8B4513;
            margin-right: 0.4cm;
            width: 1.2cm;
            height: 1.2cm;
            background: linear-gradient(135deg, rgba(139, 69, 19, 0.1) 0%, rgba(210, 180, 140, 0.1) 100%);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        
        .card-title {
            font-size: 1.1rem;
            color: #5D2E1F;
            font-weight: bold;
        }
        
        .card-subtitle {
            font-size: 0.75rem;
            color: #8B4513;
            margin-top: 0.15cm;
            opacity: 0.8;
        }
        
        /* 玉玉流派专用布局 */
        .yuyu-section {
            margin-top: 0.5cm;
        }
        
        .yuyu-header {
            text-align: center;
            margin-bottom: 0.6cm;
            padding: 0.4cm;
            background: linear-gradient(135deg, rgba(139, 69, 19, 0.05) 0%, rgba(139, 69, 19, 0.1) 100%);
            border-radius: 0.2cm;
            border-left: 0.1cm solid #8B4513;
        }
        
        .yuyu-header h3 {
            color: #5D2E1F;
            font-size: 0.9rem;
            margin-bottom: 0.15cm;
        }
        
        .yuyu-header p {
            color: #8B4513;
            font-size: 0.75rem;
        }
        
        /* 策略网格布局 */
        .strategy-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 0.4cm;
            margin-top: 0.5cm;
        }
        
        @media (max-width: 768px) {
            .strategy-grid {
                grid-template-columns: 1fr;
            }
        }
        
        .strategy-item {
            background: #fff;
            border-radius: 0.2cm;
            padding: 0.5cm;
            border: 0.03cm solid rgba(139, 69, 19, 0.15);
            page-break-inside: avoid;
        }
        
        .strategy-icon {
            font-size: 0.9rem;
            color: #8B4513;
            margin-bottom: 0.3cm;
            width: 1cm;
            height: 1cm;
            background: rgba(139, 69, 19, 0.08);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        
        .strategy-title {
            font-size: 0.85rem;
            color: #5D2E1F;
            font-weight: bold;
            margin-bottom: 0.25cm;
            padding-bottom: 0.2cm;
            border-bottom: 0.05cm solid rgba(139, 69, 19, 0.2);
        }
        
        .strategy-content {
            color: #5a4a32;
            line-height: 1.5;
            font-size: 0.75rem;
        }
        
        .strategy-content ul {
            padding-left: 0.5cm;
            margin-top: 0.25cm;
        }
        
        .strategy-content li {
            margin-bottom: 0.2cm;
            position: relative;
        }
        
        .strategy-content li::before {
            content: "•";
            color: #8B4513;
            font-weight: bold;
            position: absolute;
            left: -0.3cm;
        }
        
        /* 标签样式 */
        .tag {
            display: inline-block;
            padding: 0.15cm 0.3cm;
            background: linear-gradient(135deg, rgba(139, 69, 19, 0.1) 0%, rgba(210, 180, 140, 0.1) 100%);
            border-radius: 0.5cm;
            font-size: 0.7rem;
            color: #5D2E1F;
            font-weight: 500;
            border: 0.03cm solid rgba(139, 69, 19, 0.2);
        }
        
        /* 连招列表 */
        .combo-list {
            list-style-type: none;
            counter-reset: combo-counter;
            margin-top: 0.5cm;
        }
        
        .combo-list li {
            counter-increment: combo-counter;
            margin-bottom: 0.5cm;
            padding-left: 1.2cm;
            position: relative;
            padding-top: 0.1cm;
        }
        
        .combo-list li::before {
            content: counter(combo-counter);
            position: absolute;
            left: 0;
            top: 0;
            width: 0.9cm;
            height: 0.9cm;
            background: linear-gradient(135deg, #8B4513 0%, #D2B48C 100%);
            color: white;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: bold;
            font-size: 0.75rem;
        }
        
        .combo-sequence {
            font-family: 'Courier New', monospace;
            background: linear-gradient(135deg, rgba(139, 69, 19, 0.05) 0%, rgba(139, 69, 19, 0.1) 100%);
            padding: 0.25cm 0.4cm;
            border-radius: 0.15cm;
            display: inline-block;
            margin: 0.2cm 0;
            font-weight: bold;
            color: #5D2E1F;
            border-left: 0.1cm solid #8B4513;
            font-size: 0.8rem;
        }
        
        /* 提示框 */
        .tip-box {
            background: linear-gradient(135deg, rgba(210, 180, 140, 0.1) 0%, rgba(139, 69, 19, 0.05) 100%);
            border-left: 0.1cm solid #8B4513;
            padding: 0.5cm;
            margin: 0.6cm 0;
            border-radius: 0 0.2cm 0.2cm 0;
        }
        
        .tip-title {
            font-weight: bold;
            color: #5D2E1F;
            margin-bottom: 0.25cm;
            display: flex;
            align-items: center;
            font-size: 0.8rem;
        }
        
        .tip-title i {
            margin-right: 0.25cm;
            color: #8B4513;
            font-size: 0.8rem;
        }
        
        /* 页脚 */
        .footer {
            text-align: center;
            margin-top: 1.5cm;
            padding-top: 0.8cm;
            border-top: 0.03cm solid rgba(139, 69, 19, 0.2);
            color: #8B4513;
            font-size: 0.7rem;
            width: 100%;
            page-break-before: avoid;
        }
        
        .print-btn {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            background: linear-gradient(135deg, #8B4513 0%, #D2B48C 100%);
            color: white;
            padding: 0.3cm 0.8cm;
            border-radius: 0.5cm;
            text-decoration: none;
            margin-top: 0.5cm;
            transition: all 0.3s ease;
            border: none;
            cursor: pointer;
            font-family: inherit;
            font-size: 0.8rem;
            font-weight: bold;
        }
        
        .print-btn i {
            margin-right: 0.2cm;
        }
        
        /* 打印时隐藏按钮 */
        @media print {
            .print-btn, .no-print {
                display: none !important;
            }
            
            .card {
                box-shadow: none !important;
                border: 0.03cm solid #ddd !important;
            }
            
            .header-section {
                box-shadow: none !important;
            }
        }
        
        /* 强调文本 */
        .emphasis {
            color: #8B4513;
            font-weight: bold;
            background: rgba(139, 69, 19, 0.1);
            padding: 0.05cm 0.15cm;
            border-radius: 0.1cm;
        }
        
        /* 技能高亮 */
        .skill {
            color: #8B1A1A;
            font-weight: bold;
            font-style: italic;
        }
        
        /* 对战强度指示器 */
        .matchup-rating {
            display: inline-flex;
            align-items: center;
            margin-left: 0.25cm;
        }
        
        .star {
            color: #FFD700;
            margin-right: 0.05cm;
            font-size: 0.7rem;
        }
        
        .star.empty {
            color: #E0E0E0;
        }
        
        /* 响应式设计 */
        @media (max-width: 21cm) {
            .strategy-grid {
                grid-template-columns: 1fr;
            }
            
            .card {
                padding: 0.6cm;
            }
            
            .combo-list li {
                padding-left: 1cm;
            }
            
            .combo-list li::before {
                width: 0.8cm;
                height: 0.8cm;
            }
        }
        
        /* 水印效果 */
        .watermark {
            position: fixed;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%) rotate(-45deg);
            font-size: 8rem;
            color: rgba(139, 69, 19, 0.03);
            z-index: -1;
            white-space: nowrap;
            pointer-events: none;
        }
    </style>
</head>
<body>
    <!-- 水印 -->
    <div class="watermark">燕云十六声 2026</div>
    
    <div class="main-container">
        <!-- 页眉部分 -->
        <div class="header-section">
            <h1>鸣金虹流派PVP完全攻略</h1>
            <div class="subtitle">水墨江湖 · 剑影枪芒 · 赛季制霸指南</div>
            
            <div class="header-tags">
                <span class="tag">版本：2026.12赛季</span>
                <span class="tag">适用：PVP竞技</span>
                <span class="tag">难度：★★★★☆</span>
                <span class="tag">更新：2026.12</span>
                <span class="tag">作者：深度体验玩家</span>
            </div>
        </div>
        
        <!-- 核心装备卡片 -->
        <div class="card-container">
            <div class="card">
                <div class="card-header">
                    <div class="card-icon">
                        <i class="fas fa-helmet-battle"></i>
                    </div>
                    <div>
                        <div class="card-title">核心装备配置</div>
                        <div class="card-subtitle">金色定音 · 属性优先级 · 流派适配</div>
                    </div>
                </div>
                
                <p style="font-size: 0.8rem; margin-bottom: 0.4cm;"><strong>核心思路：</strong>以<strong>金色定音</strong>套装为基础，构建高续航、强解场、善反打的综合能力。</p>
                
                <div class="tip-box">
                    <div class="tip-title"><i class="fas fa-lightbulb"></i> 配置要诀</div>
                    <p style="font-size: 0.75rem;">优先保证<strong>解控强韧</strong>和<strong>伤害减免</strong>的生存属性，再根据对战流派微调输出属性。腕甲的"连续卸造成伤害增加"在对抗高频卸势流派时有奇效。</p>
                </div>
            </div>
        </div>
        
        <!-- 玉玉流派专项卡片 -->
        <div class="card-container">
            <div class="card">
                <div class="card-header">
                    <div class="card-icon">
                        <i class="fas fa-user-ninja"></i>
                    </div>
                    <div>
                        <div class="card-title">专项应对：玉玉流派</div>
                        <div class="card-subtitle">挑飞克制 · 解控时机 · 节奏掌控 · 完全解析</div>
                    </div>
                </div>
                
                <div class="yuyu-header">
                    <h3>核心威胁：挑飞技（两段判定）</h3>
                    <p>玉玉流派以强控制和高爆发著称，掌握应对策略是鸣金虹上分的关键</p>
                    <div class="matchup-rating">
                        <span class="emphasis">对战强度：</span>
                        <span class="star"><i class="fas fa-star"></i></span>
                        <span class="star"><i class="fas fa-star"></i></span>
                        <span class="star"><i class="fas fa-star"></i></span>
                        <span class="star"><i class="fas fa-star"></i></span>
                        <span class="star empty"><i class="fas fa-star"></i></span>
                        <span style="margin-left: 0.2cm; color: #5D2E1F; font-size: 0.7rem;">(4/5 星)</span>
                    </div>
                </div>
                
                <div class="strategy-grid">
                    <div class="strategy-item">
                        <div class="strategy-icon">
                            <i class="fas fa-shield-alt"></i>
                        </div>
                        <div class="strategy-title">防御策略</div>
                        <div class="strategy-content">
                            <p>针对玉玉的挑飞技能，需根据距离调整防御方式：</p>
                            <ul>
                                <li><span class="emphasis">远距离：</span>提前捏住格挡，预判挑飞</li>
                                <li><span class="emphasis">近距离：</span>观察技能前摇，精准格挡</li>
                                <li><span class="emphasis">应对挑飞：</span>挑飞有两段判定，使用卸势需按两下，格挡则需持续按住</li>
                            </ul>
                        </div>
                    </div>
                    
                    <div class="strategy-item">
                        <div class="strategy-icon">
                            <i class="fas fa-bolt"></i>
                        </div>
                        <div class="strategy-title">打断技巧</div>
                        <div class="strategy-content">
                            <p>有效打断玉玉技能链的关键方法：</p>
                            <ul>
                                <li><span class="skill">风墙</span>可打断非强韧技能</li>
                                <li>使用<span class="skill">骑龙</span>抓对手落地时机（时机要求高）</li>
                                <li>强韧技能和特定奇术可顶掉部分控制</li>
                                <li>提前预判对手技能释放节奏，抢先手打断</li>
                            </ul>
                        </div>
                    </div>
                    
                    <div class="strategy-item">
                        <div class="strategy-icon">
                            <i class="fas fa-clock"></i>
                        </div>
                        <div class="strategy-title">解控时机</div>
                        <div class="strategy-content">
                            <p>解控是应对玉玉的关键，时机选择至关重要：</p>
                            <ul>
                                <li><span class="emphasis">只解抛春恨：</span>这是玉玉的核心控制技能</li>
                                <li><span class="emphasis">近距离：</span>立即解控可造成僵直，创造反击机会</li>
                                <li><span class="emphasis">远距离：</span>可故意吃一次抛春恨再解，骗对手技能</li>
                                <li>避免在非关键控制上浪费解控技能</li>
                            </ul>
                        </div>
                    </div>
                    
                    <div class="strategy-item">
                        <div class="strategy-icon">
                            <i class="fas fa-running"></i>
                        </div>
                        <div class="strategy-title">抛春恨应对</div>
                        <div class="strategy-content">
                            <p>针对玉玉的核心技能"抛春恨"的应对策略：</p>
                            <ul>
                                <li><span class="emphasis">远距离：</span>左右闪避，保持移动</li>
                                <li><span class="emphasis">近距离：</span>前闪贴近对手，抓反击时机</li>
                                <li>观察对手释放习惯，预判抛春恨时机</li>
                                <li>被命中后根据距离决定是否立即解控</li>
                            </ul>
                        </div>
                    </div>
                    
                    <div class="strategy-item">
                        <div class="strategy-icon">
                            <i class="fas fa-gamepad"></i>
                        </div>
                        <div class="strategy-title">开局处理</div>
                        <div class="strategy-content">
                            <p>开局阶段奠定整局对战基调：</p>
                            <ul>
                                <li>对手开局喝酒时，必用卸势打断</li>
                                <li>对方使用钧钧开局时，不要轻易套buff，容易吃抛春恨</li>
                                <li>开局优先观察对手技能释放习惯</li>
                                <li>试探性进攻，了解对手反应模式</li>
                            </ul>
                        </div>
                    </div>
                    
                    <div class="strategy-item">
                        <div class="strategy-icon">
                            <i class="fas fa-tachometer-alt"></i>
                        </div>
                        <div class="strategy-title">节奏掌控</div>
                        <div class="strategy-content">
                            <p>掌握对战节奏是取胜的关键：</p>
                            <ul>
                                <li><span class="emphasis">有解控时：</span>主动施压，避免远程周旋</li>
                                <li><span class="emphasis">无解控时：</span>暂缓节奏，等待技能冷却</li>
                                <li>对奇术大师型玉玉，不要轻易卸蛤蟆</li>
                                <li>持续给予压力，不让对手轻松控制战局</li>
                            </ul>
                        </div>
                    </div>
                </div>
                
                <div class="tip-box">
                    <div class="tip-title"><i class="fas fa-lightbulb"></i> 高级应对技巧</div>
                    <p style="font-size: 0.75rem;"><span class="emphasis">奇术应对：</span>面对奇术大师型玉玉，不要轻易卸蛤蟆，除非确认能反吃药叉。</p>
                    <p style="font-size: 0.75rem; margin-top: 0.2cm;"><span class="emphasis">心理博弈：</span>和玉玉打要给持续压力，有解控时不要远程周旋，没解控就缓一缓节奏，等待机会。</p>
                    <p style="font-size: 0.75rem; margin-top: 0.2cm;"><span class="emphasis">技能预判：</span>玉玉的挑飞技能前摇明显，通过大量练习可以做到精准格挡或闪避。</p>
                </div>
            </div>
        </div>
        
        <!-- 其他核心策略卡片 -->
        <div class="card-container">
            <!-- 风风流派 -->
            <div class="card">
                <div class="card-header">
                    <div class="card-icon">
                        <i class="fas fa-wind"></i>
                    </div>
                    <div>
                        <div class="card-title">应对：风风流派</div>
                        <div class="card-subtitle">蓄力老鼠版本 · 打断技巧 · 藏招策略</div>
                    </div>
                </div>
                
                <div class="yuyu-header">
                    <h3>蓄力老鼠版本应对</h3>
                    <p>风风流派依赖蓄力技能，重点在于打断节奏</p>
                </div>
                
                <ul class="combo-list">
                    <li>
                        <strong>开局反制：</strong>
                        <div class="combo-sequence">燕返 + 蓄力打断 或 直接使用凌云踏</div>
                        <p style="font-size: 0.75rem;">利用突进技能打断对手蓄力，抢占先机</p>
                    </li>
                    <li>
                        <strong>近身策略：</strong>
                        <p style="font-size: 0.75rem;">藏<span class="skill">气涌</span>接近对手，可藏<span class="skill">药叉</span>（若药茶成功则接蛤蟆）</p>
                    </li>
                    <li>
                        <strong>爆发时机：</strong>
                        <div class="combo-sequence">处决后接吐火</div>
                        <p style="font-size: 0.75rem;">处决后立即接吐火，最大化伤害输出</p>
                    </li>
                    <li>
                        <strong>防守反击：</strong>
                        <p style="font-size: 0.75rem;">对手砖过来时预判<span class="skill">吐火</span>，或使用火拳应对</p>
                    </li>
                </ul>
                
                <div class="tip-box">
                    <div class="tip-title"><i class="fas fa-brain"></i> 对战思路</div>
                    <p style="font-size: 0.75rem;">风风流派依赖蓄力技能，重点在于打断其蓄力节奏。利用燕返和凌云踏的突进能力保持压迫，不给其安全蓄力的空间。</p>
                </div>
            </div>
            
            <!-- 其他流派要点 -->
            <div class="card">
                <div class="card-header">
                    <div class="card-icon">
                        <i class="fas fa-users"></i>
                    </div>
                    <div>
                        <div class="card-title">其他流派应对要点</div>
                        <div class="card-subtitle">快速查阅 · 核心技巧 · 注意事项</div>
                    </div>
                </div>
                
                <div class="strategy-item" style="margin-bottom: 0.5cm; border-left: 0.1cm solid #8B4513;">
                    <div class="strategy-title">威威流派</div>
                    <div class="strategy-content">
                        <ul>
                            <li>提前喝酒保证状态</li>
                            <li><span class="combo-sequence">无名枪定身 + 吐火</span> 形成连招</li>
                            <li>遇到善卸势的对手，不要轻易放剑气，或尝试剑气藏药茶</li>
                        </ul>
                    </div>
                </div>
                
                <div class="strategy-item" style="margin-bottom: 0.5cm; border-left: 0.1cm solid #8B4513;">
                    <div class="strategy-title">影影流派</div>
                    <div class="strategy-content">
                        <ul>
                            <li>核心：卸掉对手99的武学技</li>
                            <li>输出循环：<span class="combo-sequence">燕返 + 蓄力输出</span></li>
                            <li>用<span class="skill">9剑蓄力</span>追击或拉开距离</li>
                            <li>Q卸QQ，重击两次后接蛤蟆</li>
                        </ul>
                    </div>
                </div>
                
                <div class="strategy-item" style="margin-bottom: 0.5cm; border-left: 0.1cm solid #8B4513;">
                    <div class="strategy-title">虹虹流派</div>
                    <div class="strategy-content">
                        <ul>
                            <li>警惕气涌藏药茶</li>
                            <li>若卸不净剑气，可改用格挡</li>
                            <li>近身博弈：躲避乾坤定，抓对手易武后摇</li>
                            <li>注意20秒气涌周期，长时间拉扯需提防</li>
                        </ul>
                    </div>
                </div>
                
                <div class="tip-box">
                    <div class="tip-title"><i class="fas fa-clipboard-list"></i> 通用对战原则</div>
                    <p style="font-size: 0.75rem;">1. 关键技能（药茶、气涌）尽量藏在连招中<br>
                       2. 时刻关注真气、耐力、解控CD<br>
                       3. 根据自身技能状态决定进攻或拉扯节奏<br>
                       4. 观察对手习惯，针对性调整策略</p>
                </div>
            </div>
        </div>
        
        <!-- 页脚 -->
        <div class="footer">
            <p><strong>《燕云十六声》鸣金虹流派PVP完全攻略 | 适用于2026.12赛季版本</strong></p>
            <p style="margin-top: 0.3cm;">本攻略由深度玩家基于1000+小时实战经验总结，仅供参考，实际对战请灵活应变</p>
            
            <div class="no-print">
                <button class="print-btn" onclick="printPDF()">
                    <i class="fas fa-file-pdf"></i> 导出为PDF
                </button>
                <p style="margin-top: 0.4cm; font-size: 0.65rem; color: #8B4513;">导出提示：点击上方按钮或使用Ctrl+P，在打印设置中选择"另存为PDF"</p>
            </div>
            
            <p style="margin-top: 0.8cm; color: #A0522D; font-size: 0.65rem; border-top: 0.03cm solid rgba(139, 69, 19, 0.2); padding-top: 0.4cm;">
                © 2026 玩家体验 | 本攻略仅供学习交流使用 | 更新时间：2026年12月
            </p>
        </div>
    </div>
    
    <script>
        // 打印为PDF
        function printPDF() {
            window.print();
        }
        
        // 页面加载后自动调整打印样式
        document.addEventListener('DOMContentLoaded', function() {
            // 打印时添加页眉页脚
            const style = document.createElement('style');
            style.textContent = `
                @media print {
                    @page {
                        @top-center {
                            content: "《燕云十六声》鸣金虹PVP攻略";
                            font-size: 10pt;
                            color: #8B4513;
                        }
                        @bottom-center {
                            content: "第" counter(page) "页 / 共" counter(pages) "页";
                            font-size: 9pt;
                            color: #8B4513;
                        }
                    }
                }
            `;
            document.head.appendChild(style);
        });
    </script>
</body>
</html>
