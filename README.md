<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>اختبار الرخصة المهنية التفاعلي | إعداد: فهد الخالدي</title>
    <meta name="description" content="اختبار الرخصة المهنية التفاعلي للمعلمين - إعداد المعلم فهد الخالدي">
    <link href="https://fonts.googleapis.com/css2?family=Tajawal:wght@300;400;500;700;800&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            /* ألوان متطورة وجذابة */
            --primary: #6366F1;
            --primary-dark: #4F46E5;
            --primary-light: #8B5CF6;
            --accent: #EC4899;
            --accent-dark: #DB2777;
            --accent-light: #F472B6;
            --secondary: #10B981;
            --secondary-dark: #059669;
            --tertiary: #F59E0B;
            --quaternary: #8B5CF6;
            --bg: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            --card-bg: rgba(255, 255, 255, 0.95);
            --text: #1F2937;
            --light-text: #6B7280;
            --border: rgba(255, 255, 255, 0.2);
            --shadow: 0 8px 32px rgba(0, 0, 0, 0.1);
            --shadow-hover: 0 20px 40px rgba(0, 0, 0, 0.2);
            --gradient: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            --gradient-dark: linear-gradient(135deg, #5a67d8 0%, #6b46c1 100%);
            --gradient-light: linear-gradient(135deg, #a78bfa 0%, #c4b5fd 100%);
            --accent-gradient: linear-gradient(135deg, #EC4899, #8B5CF6);
            --success-gradient: linear-gradient(135deg, #10B981, #34D399);
            --warning-gradient: linear-gradient(135deg, #F59E0B, #FBBF24);
            --primary-gradient: linear-gradient(135deg, #6366F1, #8B5CF6);
        }

        .dark-theme {
            --bg: linear-gradient(135deg, #1e3c72 0%, #2a5298 100%);
            --card-bg: rgba(30, 41, 59, 0.95);
            --text: #F1F5F9;
            --light-text: #CBD5E1;
            --border: rgba(255, 255, 255, 0.1);
            --shadow: 0 8px 32px rgba(0, 0, 0, 0.3);
            --shadow-hover: 0 20px 40px rgba(0, 0, 0, 0.4);
        }

        * {
            box-sizing: border-box;
            font-family: 'Tajawal', Tahoma, Arial, sans-serif;
            margin: 0;
            padding: 0;
        }

        body {
            background: var(--bg);
            color: var(--text);
            line-height: 1.7;
            overflow-x: hidden;
            padding-top: 80px;
            transition: all 0.5s ease;
            min-height: 100vh;
        }

        /* Header بتصميم شفاف وجذاب */
        header {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(20px);
            color: white;
            position: fixed;
            top: 0;
            width: 100%;
            z-index: 1000;
            box-shadow: var(--shadow);
            border-bottom: 1px solid var(--border);
            padding: 15px 0;
        }

        .header-container {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 0 20px;
        }

        .title-section h1 {
            font-size: 1.5rem;
            font-weight: 800;
            background: var(--accent-gradient);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            text-shadow: 0 2px 10px rgba(236, 72, 153, 0.3);
        }

        .header-actions {
            display: flex;
            gap: 10px;
        }

        .theme-btn, .back-btn {
            background: rgba(255, 255, 255, 0.15);
            color: white;
            border: 1px solid rgba(255, 255, 255, 0.2);
            padding: 8px 15px;
            border-radius: 12px;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
            display: flex;
            align-items: center;
            gap: 6px;
            backdrop-filter: blur(10px);
            text-decoration: none;
        }

        .theme-btn:hover, .back-btn:hover {
            background: rgba(255, 255, 255, 0.25);
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }

        /* Main Content */
        main {
            max-width: 1000px;
            margin: 30px auto;
            padding: 0 20px;
        }

        .hero-section {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(20px);
            color: white;
            border-radius: 24px;
            padding: 40px;
            margin-bottom: 30px;
            text-align: center;
            position: relative;
            overflow: hidden;
            box-shadow: var(--shadow);
            border: 1px solid var(--border);
        }

        .hero-section::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: var(--accent-gradient);
            opacity: 0.1;
            z-index: -1;
        }

        .hero-content {
            position: relative;
            z-index: 1;
        }

        .hero-title {
            font-size: 2.2rem;
            font-weight: 800;
            margin-bottom: 15px;
            background: linear-gradient(135deg, #fff 0%, #f0f0f0 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .hero-subtitle {
            font-size: 1.1rem;
            margin-bottom: 25px;
            opacity: 0.9;
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
        }

        /* Cards بتصميم زجاجي */
        .card {
            background: var(--card-bg);
            backdrop-filter: blur(20px);
            border-radius: 20px;
            padding: 30px;
            margin-bottom: 25px;
            box-shadow: var(--shadow);
            transition: all 0.4s ease;
            border: 1px solid var(--border);
            position: relative;
            overflow: hidden;
        }

        .card::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 4px;
            background: var(--accent-gradient);
        }

        .card:hover {
            transform: translateY(-8px) scale(1.02);
            box-shadow: var(--shadow-hover);
        }

        .section-title {
            text-align: center;
            color: var(--text);
            margin-bottom: 30px;
            font-size: 2rem;
            font-weight: 800;
            position: relative;
            padding-bottom: 15px;
        }

        .section-title::after {
            content: "";
            position: absolute;
            bottom: 0;
            right: 50%;
            transform: translateX(50%);
            width: 100px;
            height: 4px;
            background: var(--accent-gradient);
            border-radius: 2px;
        }

        /* تصميم الأسئلة المتطور */
        .question-box {
            background: var(--card-bg);
            backdrop-filter: blur(20px);
            padding: 30px;
            margin-bottom: 25px;
            border-radius: 20px;
            box-shadow: var(--shadow);
            border: 1px solid var(--border);
            transition: all 0.4s ease;
            position: relative;
            overflow: hidden;
        }

        .question-box::before {
            content: "";
            position: absolute;
            top: 0;
            right: 0;
            width: 100%;
            height: 5px;
            background: var(--primary-gradient);
        }

        .question-box:hover {
            transform: translateY(-5px);
            box-shadow: var(--shadow-hover);
        }

        .question-number {
            font-size: 1.3em;
            color: var(--primary);
            margin-bottom: 15px;
            font-weight: bold;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .question-number i {
            color: var(--accent);
            font-size: 1.2em;
        }

        .question-text {
            font-size: 1.2em;
            margin-bottom: 25px;
            line-height: 1.7;
            color: var(--text);
            font-weight: 500;
        }

        .options {
            position: relative;
        }

        .options label {
            display: flex;
            align-items: center;
            padding: 18px 20px;
            margin: 12px 0;
            border: 2px solid var(--border);
            border-radius: 15px;
            cursor: pointer;
            transition: all 0.3s ease;
            background: var(--card-bg);
            position: relative;
            overflow: hidden;
            font-weight: 500;
        }

        .options label::before {
            content: "";
            position: absolute;
            left: 0;
            top: 0;
            height: 100%;
            width: 0;
            background: var(--primary-gradient);
            transition: width 0.3s ease;
            z-index: 0;
        }

        .options label:hover {
            border-color: var(--primary);
            transform: translateX(-8px);
            box-shadow: 0 5px 15px rgba(99, 102, 241, 0.2);
        }

        .options label:hover::before {
            width: 4px;
        }

        .options input[type="radio"] {
            margin-left: 12px;
            transform: scale(1.3);
            z-index: 1;
        }

        /* عندما تكون الإجابة مقفولة */
        .options label.locked {
            cursor: not-allowed;
            opacity: 0.8;
        }

        .options label.selected {
            background: linear-gradient(135deg, rgba(99, 102, 241, 0.1), rgba(139, 92, 246, 0.1));
            border-color: var(--primary);
            box-shadow: 0 5px 15px rgba(99, 102, 241, 0.2);
        }

        .options label.selected::before {
            width: 6px;
            background: var(--success-gradient);
        }

        .options label.correct-answer {
            background: linear-gradient(135deg, rgba(16, 185, 129, 0.15), rgba(52, 211, 153, 0.15));
            border-color: var(--secondary);
            box-shadow: 0 5px 15px rgba(16, 185, 129, 0.2);
        }

        .options label.correct-answer::before {
            width: 6px;
            background: var(--success-gradient);
        }

        .options label.wrong-answer {
            background: linear-gradient(135deg, rgba(236, 72, 153, 0.1), rgba(244, 114, 182, 0.1));
            border-color: var(--accent);
            box-shadow: 0 5px 15px rgba(236, 72, 153, 0.2);
        }

        .options label.wrong-answer::before {
            width: 6px;
            background: var(--accent-gradient);
        }

        .correct {
            color: var(--secondary);
            font-weight: bold;
        }

        .wrong {
            color: var(--accent);
            font-weight: bold;
        }

        .explanation {
            margin-top: 25px;
            padding: 25px;
            border-radius: 15px;
            display: none;
            background: linear-gradient(135deg, rgba(99, 102, 241, 0.05), rgba(236, 72, 153, 0.05));
            border-left: 4px solid var(--secondary);
            animation: slideDown 0.5s ease;
            backdrop-filter: blur(10px);
        }

        @keyframes slideDown {
            from {
                opacity: 0;
                transform: translateY(-15px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .explanation-line {
            padding: 15px;
            margin: 10px 0;
            border-radius: 10px;
            transition: all 0.3s ease;
        }

        .explanation-correct {
            background: linear-gradient(135deg, rgba(16, 185, 129, 0.1), rgba(52, 211, 153, 0.1));
            border-right: 3px solid var(--secondary);
        }

        .explanation-wrong-1 {
            background: linear-gradient(135deg, rgba(236, 72, 153, 0.1), rgba(244, 114, 182, 0.1));
            border-right: 3px solid var(--accent);
        }

        .explanation-wrong-2 {
            background: linear-gradient(135deg, rgba(245, 158, 11, 0.1), rgba(251, 191, 36, 0.1));
            border-right: 3px solid var(--tertiary);
        }

        .explanation-wrong-3 {
            background: linear-gradient(135deg, rgba(139, 92, 246, 0.1), rgba(196, 181, 253, 0.1));
            border-right: 3px solid var(--quaternary);
        }

        /* Navigation Buttons */
        .navigation {
            display: flex;
            justify-content: space-between;
            margin-top: 30px;
            gap: 20px;
        }

        .btn {
            padding: 15px 30px;
            border-radius: 15px;
            font-weight: 700;
            text-decoration: none;
            transition: all 0.3s ease;
            display: inline-flex;
            align-items: center;
            gap: 10px;
            font-size: 1rem;
            border: none;
            cursor: pointer;
            position: relative;
            overflow: hidden;
        }

        .btn::before {
            content: "";
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255,255,255,0.3), transparent);
            transition: left 0.6s;
        }

        .btn:hover::before {
            left: 100%;
        }

        .btn-primary {
            background: var(--accent-gradient);
            color: white;
            box-shadow: 0 8px 25px rgba(236, 72, 153, 0.3);
        }

        .btn-primary:hover {
            transform: translateY(-5px) scale(1.05);
            box-shadow: 0 15px 35px rgba(236, 72, 153, 0.4);
        }

        .btn-secondary {
            background: var(--primary-gradient);
            color: white;
            box-shadow: 0 8px 25px rgba(99, 102, 241, 0.3);
        }

        .btn-secondary:hover {
            transform: translateY(-5px) scale(1.05);
            box-shadow: 0 15px 35px rgba(99, 102, 241, 0.4);
        }

        .btn:disabled {
            background: #9CA3AF;
            cursor: not-allowed;
            transform: none;
            box-shadow: none;
        }

        .btn:disabled:hover::before {
            left: -100%;
        }

        /* Progress Bar متطور */
        .progress-bar {
            height: 15px;
            background: rgba(255, 255, 255, 0.2);
            border-radius: 10px;
            margin-bottom: 30px;
            overflow: hidden;
            box-shadow: inset 0 2px 5px rgba(0, 0, 0, 0.1);
            position: relative;
            backdrop-filter: blur(10px);
        }

        .progress {
            height: 100%;
            background: var(--accent-gradient);
            width: 0%;
            transition: width 0.5s ease;
            border-radius: 10px;
            position: relative;
            overflow: hidden;
        }

        .progress::after {
            content: "";
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255,255,255,0.4), transparent);
            animation: shimmer 1.5s infinite;
        }

        @keyframes shimmer {
            0% { left: -100%; }
            100% { left: 100%; }
        }

        /* Results Box */
        #result-box, #current-score {
            background: var(--card-bg);
            backdrop-filter: blur(20px);
            padding: 30px;
            margin-top: 30px;
            border-radius: 20px;
            box-shadow: var(--shadow);
            border: 1px solid var(--border);
            display: none;
            animation: slideUp 0.6s ease;
        }

        @keyframes slideUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .controls {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-top: 30px;
            flex-wrap: wrap;
            gap: 20px;
        }

        .quiz-info {
            font-size: 1rem;
            color: var(--light-text);
            background: linear-gradient(135deg, rgba(99, 102, 241, 0.1), rgba(236, 72, 153, 0.1));
            padding: 10px 20px;
            border-radius: 25px;
            font-weight: 600;
            backdrop-filter: blur(10px);
        }

        /* Timer متطور */
        #timer {
            font-size: 1.1rem;
            font-weight: bold;
            color: white;
            margin-left: 20px;
            display: flex;
            align-items: center;
            gap: 8px;
            background: rgba(255, 255, 255, 0.2);
            padding: 10px 20px;
            border-radius: 25px;
            backdrop-filter: blur(10px);
        }

        .timer-warning {
            color: #FECACA !important;
            animation: pulse 0.8s infinite;
            background: rgba(254, 202, 202, 0.3) !important;
        }

        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.05); }
            100% { transform: scale(1); }
        }

        /* Questions List متطور */
        #questions-list {
            margin-top: 25px;
            background: var(--card-bg);
            backdrop-filter: blur(20px);
            padding: 30px;
            border-radius: 20px;
            box-shadow: var(--shadow);
            border: 1px solid var(--border);
            display: none;
        }

        #questions-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(60px, 1fr));
            gap: 12px;
            margin: 20px 0;
        }

        .question-status-grid {
            width: 60px;
            height: 60px;
            border: 2px solid var(--border);
            border-radius: 15px;
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            font-weight: 700;
            transition: all 0.3s ease;
            background: var(--card-bg);
            position: relative;
            overflow: hidden;
            font-size: 1.1rem;
        }

        .question-status-grid::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: var(--accent-gradient);
            opacity: 0;
            transition: opacity 0.3s ease;
        }

        .question-status-grid:hover {
            transform: translateY(-3px) scale(1.1);
            box-shadow: var(--shadow);
        }

        .question-status-grid.current {
            border-color: var(--accent);
            background: var(--accent);
            color: white;
            transform: scale(1.1);
        }

        .question-status-grid.answered {
            border-color: var(--secondary);
            background: var(--secondary);
            color: white;
        }

        .question-status-grid.flagged {
            border-color: var(--tertiary);
            background: var(--tertiary);
            color: var(--text);
        }

        .question-status-grid span {
            position: relative;
            z-index: 1;
        }

        .legend {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            margin-top: 20px;
            font-size: 0.9rem;
        }

        .legend-item {
            display: flex;
            align-items: center;
            gap: 10px;
        }

        /* تحسينات للوضع الداكن */
        .dark-theme .question-status-grid {
            border-color: var(--border);
        }

        .dark-theme .options label {
            background: var(--card-bg);
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            body {
                padding-top: 70px;
            }
            
            .header-container {
                padding: 0 15px;
                flex-direction: column;
                gap: 15px;
            }
            
            .title-section h1 {
                font-size: 1.3rem;
            }
            
            .hero-title {
                font-size: 1.8rem;
            }
            
            .hero-subtitle {
                font-size: 1rem;
            }
            
            .card, .question-box {
                padding: 25px;
            }
            
            .navigation {
                flex-direction: column;
                gap: 15px;
            }
            
            .btn {
                width: 100%;
                justify-content: center;
            }
            
            .controls {
                flex-direction: column;
                align-items: stretch;
            }
            
            #questions-grid {
                grid-template-columns: repeat(auto-fill, minmax(50px, 1fr));
            }
            
            .question-status-grid {
                width: 50px;
                height: 50px;
                font-size: 1rem;
            }
        }

        @media (max-width: 480px) {
            .header-container {
                text-align: center;
            }
            
            .header-actions {
                justify-content: center;
            }
            
            .question-box {
                padding: 20px;
            }
            
            .options label {
                padding: 15px;
            }
            
            .hero-section {
                padding: 25px;
            }
            
            .section-title {
                font-size: 1.6rem;
            }
        }

        /* تأثيرات إضافية */
        .fade-in {
            animation: fadeIn 0.8s ease;
        }

        @keyframes fadeIn {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .bounce-in {
            animation: bounceIn 0.8s ease;
        }

        @keyframes bounceIn {
            0% {
                opacity: 0;
                transform: scale(0.3);
            }
            50% {
                opacity: 1;
                transform: scale(1.05);
            }
            70% {
                transform: scale(0.95);
            }
            100% {
                opacity: 1;
                transform: scale(1);
            }
        }

        /* تأثيرات الجلاس مورفيزم */
        .glass-effect {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(20px);
            border: 1px solid rgba(255, 255, 255, 0.2);
        }

        /* رسوم متحركة للخلفية */
        .bg-animation {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -1;
            opacity: 0.3;
        }

        .floating-shapes {
            position: absolute;
            width: 100%;
            height: 100%;
        }

        .shape {
            position: absolute;
            background: var(--accent-gradient);
            border-radius: 50%;
            opacity: 0.1;
            animation: float 6s ease-in-out infinite;
        }

        .shape:nth-child(1) {
            width: 100px;
            height: 100px;
            top: 10%;
            left: 10%;
            animation-delay: 0s;
        }

        .shape:nth-child(2) {
            width: 150px;
            height: 150px;
            top: 60%;
            right: 10%;
            animation-delay: 2s;
        }

        .shape:nth-child(3) {
            width: 80px;
            height: 80px;
            bottom: 20%;
            left: 20%;
            animation-delay: 4s;
        }

        @keyframes float {
            0%, 100% {
                transform: translateY(0) rotate(0deg);
            }
            50% {
                transform: translateY(-20px) rotate(180deg);
            }
        }
    </style>
</head>
<body>
    <!-- رسوم متحركة للخلفية -->
    <div class="bg-animation">
        <div class="floating-shapes">
            <div class="shape"></div>
            <div class="shape"></div>
            <div class="shape"></div>
        </div>
    </div>

    <!-- Header -->
    <header class="glass-effect">
        <div class="header-container">
            <div class="title-section">
                <h1>اختبار الرخصة المهنية التفاعلي</h1>
            </div>
            <div class="header-actions">
                <button class="theme-btn" id="themeBtn">
                    <i class="fas fa-moon"></i>
                </button>
                <a href="#" class="back-btn">
                    <i class="fas fa-arrow-right"></i>
                    العودة للرئيسية
                </a>
            </div>
        </div>
    </header>

    <!-- Main Content -->
    <main>
        <!-- Hero Section -->
        <section class="hero-section glass-effect">
            <div class="hero-content">
                <h1 class="hero-title">اختبار الرخصة المهنية للمعلمين</h1>
                <p class="hero-subtitle">تم إعداد هذا الاختبار التفاعلي لمحاكاة الاختبار الرسمي للرخصة المهنية، ويقدم تغذية راجعة فورية لجميع الإجابات</p>
                <div class="quiz-info">إعداد: المعلم فهد الخالدي</div>
            </div>
        </section>

        <!-- Progress Bar -->
        <div class="progress-bar glass-effect">
            <div class="progress" id="progress"></div>
        </div>

        <!-- Quiz Container -->
        <div id="quiz"></div>

        <!-- Controls -->
        <div class="controls">
            <div class="quiz-info" id="quiz-info"></div>
            <div id="timer">⏱️ <span id="time-display">45:00</span></div>
            <div style="display: flex; gap: 15px; flex-wrap: wrap;">
                <button class="btn btn-primary" onclick="showQuestionsList()">
                    <i class="fas fa-list"></i>
                    قائمة الأسئلة
                </button>
                <button class="btn btn-secondary" onclick="toggleMarkForReview()" id="mark-review-btn">
                    <i class="fas fa-flag"></i>
                    وضع علامة للمراجعة
                </button>
                <button class="btn btn-primary" onclick="finishQuiz()">
                    <i class="fas fa-flag-checkered"></i>
                    إنهاء الاختبار
                </button>
                <button class="btn btn-secondary" onclick="showCurrentScore()">
                    <i class="fas fa-chart-bar"></i>
                    عرض الدرجات الحالية
                </button>
            </div>
        </div>

        <!-- Questions List -->
        <div id="questions-list" class="card">
            <h3 style="color: var(--text); margin-bottom: 20px; display: flex; align-items: center; gap: 12px;">
                <i class="fas fa-th-list"></i>
                قائمة الأسئلة
            </h3>
            <div id="questions-grid"></div>
            <div class="legend">
                <div class="legend-item">
                    <div class="question-status-grid" style="background: var(--accent); color: white;"></div>
                    <span>السؤال الحالي</span>
                </div>
                <div class="legend-item">
                    <div class="question-status-grid" style="background: var(--secondary); color: white;"></div>
                    <span>تمت الإجابة</span>
                </div>
                <div class="legend-item">
                    <div class="question-status-grid" style="background: var(--tertiary); color: var(--text);"></div>
                    <span>معلم للمراجعة</span>
                </div>
                <div class="legend-item">
                    <div class="question-status-grid" style="background: var(--card-bg); border-color: var(--border);"></div>
                    <span>لم يتم الإجابة</span>
                </div>
            </div>
            <button class="btn btn-primary" onclick="hideQuestionsList()" style="margin-top:20px; width: 100%;">
                <i class="fas fa-times"></i>
                إغلاق القائمة
            </button>
        </div>

        <!-- Current Score -->
        <div id="current-score" class="card">
            <h3 style="color: var(--text); margin-bottom: 20px; display: flex; align-items: center; gap: 12px;">
                <i class="fas fa-chart-bar"></i>
                الدرجات الحالية
            </h3>
            <p id="current-correct" style="margin-bottom: 15px; font-size: 1.1rem;"></p>
            <p id="current-percentage" style="font-weight: bold; font-size: 1.3rem; color: var(--primary);"></p>
        </div>

        <!-- Final Results -->
        <div id="result-box" class="card">
            <h3 id="result" style="color: var(--text); margin-bottom: 20px;"></h3>
            <p id="percentage" style="font-size: 1.4rem; margin-bottom: 15px;"></p>
            <p id="evaluation" style="font-weight: bold; font-size: 1.3rem;"></p>
        </div>
    </main>

    <script>
        // مصفوفة الأسئلة
        const questions = [
            {
                q: "أي من الاستراتيجيات التالية تُعتبر الأكثر فعالية في تعزيز التعلم النشط لدى الطلاب؟",
                options: [
                    "التعلم القائم على المشاريع",
                    "الحفظ والتكرار",
                    "المحاضرة التقليدية",
                    "الاختبارات الدورية"
                ],
                answer: 0,
                explanations: {
                    correct: "التعلم القائم على المشاريع يشجع الطلاب على المشاركة الفعالة وربط المعرفة بالحياة الواقعية.",
                    wrong1: "الحفظ والتكرار يركز على الاستظهار ولا يعزز الفهم العميق.",
                    wrong2: "المحاضرة التقليدية تجعل الطالب متلقيًا سلبيًا للمعرفة.",
                    wrong3: "الاختبارات الدورية تقيس التحصيل ولكنها لا تعزز بالضرورة التعلم النشط."
                }
            },
            {
                q: "ما المبدأ الأساسي الذي يرتكز عليه مفهوم التمايز التعليمي؟",
                options: [
                    "مراعاة الفروق الفردية بين الطلاب",
                    "تطبيق منهج موحد على جميع الطلاب",
                    "زيادة عدد الاختبارات",
                    "تقليل عدد الطلاب في الصف"
                ],
                answer: 0,
                explanations: {
                    correct: "التمايز التعليمي يعني تكييف التدريس ليلائم احتياجات وقدرات كل طالب.",
                    wrong1: "المنهج الموحد لا يراعي الفروق الفردية بين الطلاب.",
                    wrong2: "زيادة الاختبارات لا ترتبط مباشرة بمبدأ التمايز.",
                    wrong3: "تقليل عدد الطلاب قد يساعد ولكن ليس هو المبدأ الأساسي للتمايز."
                }
            },
            // يمكن إضافة المزيد من الأسئلة هنا
        ];

        let currentQuestionIndex = 0;
        let userAnswers = Array(questions.length).fill(null);
        let timeLeft = 45 * 60; // 45 دقيقة
        let timerInterval;
        let markedQuestions = [];
        let answerLocked = Array(questions.length).fill(false); // مصفوفة لتتبع حالة القفل لكل سؤال

        // تبديل الوضع الليلي
        document.getElementById('themeBtn').addEventListener('click', function() {
            document.body.classList.toggle('dark-theme');
            const icon = this.querySelector('i');
            if (document.body.classList.contains('dark-theme')) {
                icon.classList.remove('fa-moon');
                icon.classList.add('fa-sun');
                localStorage.setItem('darkMode', 'enabled');
            } else {
                icon.classList.remove('fa-sun');
                icon.classList.add('fa-moon');
                localStorage.setItem('darkMode', 'disabled');
            }
        });

        // التحقق من تفضيل الوضع الداكن المخزن
        function checkDarkModePreference() {
            const darkMode = localStorage.getItem('darkMode');
            const icon = document.querySelector('#themeBtn i');
            
            if (darkMode === 'enabled') {
                document.body.classList.add('dark-theme');
                icon.classList.remove('fa-moon');
                icon.classList.add('fa-sun');
            } else {
                document.body.classList.remove('dark-theme');
                icon.classList.remove('fa-sun');
                icon.classList.add('fa-moon');
            }
        }

        // المؤقت
        function startTimer() {
            timerInterval = setInterval(() => {
                timeLeft--;
                updateTimerDisplay();
                
                if (timeLeft <= 0) {
                    clearInterval(timerInterval);
                    finishQuiz();
                }
            }, 1000);
        }

        function updateTimerDisplay() {
            const minutes = Math.floor(timeLeft / 60);
            const seconds = timeLeft % 60;
            const timeDisplay = document.getElementById('time-display');
            timeDisplay.textContent = `${minutes.toString().padStart(2, '0')}:${seconds.toString().padStart(2, '0')}`;
            
            if (timeLeft < 300) { // 5 دقائق
                timeDisplay.classList.add('timer-warning');
            } else {
                timeDisplay.classList.remove('timer-warning');
            }
        }

        // عرض قائمة الأسئلة
        function showQuestionsList() {
            const grid = document.getElementById('questions-grid');
            grid.innerHTML = '';
            
            questions.forEach((_, index) => {
                const btn = document.createElement('div');
                btn.className = `question-status-grid ${index === currentQuestionIndex ? 'current' : ''} ${userAnswers[index] !== null ? 'answered' : ''} ${markedQuestions.includes(index) ? 'flagged' : ''}`;
                btn.innerHTML = `<span>${index + 1}</span>`;
                btn.onclick = () => {
                    currentQuestionIndex = index;
                    loadQuiz();
                    hideQuestionsList();
                };
                grid.appendChild(btn);
            });
            
            document.getElementById('questions-list').style.display = 'block';
        }

        function hideQuestionsList() {
            document.getElementById('questions-list').style.display = 'none';
        }

        // وضع علامة للمراجعة
        function toggleMarkForReview() {
            const index = markedQuestions.indexOf(currentQuestionIndex);
            const btn = document.getElementById('mark-review-btn');
            
            if (index === -1) {
                markedQuestions.push(currentQuestionIndex);
                btn.innerHTML = '<i class="fas fa-flag"></i> إزالة العلامة';
                btn.style.background = 'var(--tertiary)';
            } else {
                markedQuestions.splice(index, 1);
                btn.innerHTML = '<i class="fas fa-flag"></i> وضع علامة للمراجعة';
                btn.style.background = 'var(--secondary)';
            }
            
            if (document.getElementById('questions-list').style.display === 'block') {
                showQuestionsList();
            }
        }

        // تحميل الاختبار
        function loadQuiz() {
            const quizDiv = document.getElementById("quiz");
            quizDiv.innerHTML = "";

            const question = questions[currentQuestionIndex];
            const isLocked = answerLocked[currentQuestionIndex];
            
            let html = `
                <div class="question-box fade-in">
                    <div class="question-number">
                        <i class="fas fa-question-circle"></i>
                        السؤال ${currentQuestionIndex + 1} من ${questions.length}
                        ${isLocked ? '<span style="color: var(--accent); margin-right: 10px;"><i class="fas fa-lock"></i> مقفل</span>' : ''}
                    </div>
                    <div class="question-text">${question.q}</div>
                    <div class="options">
            `;
            
            question.options.forEach((opt, i) => {
                const isChecked = userAnswers[currentQuestionIndex] === i;
                const isDisabled = isLocked;
                let labelClass = '';
                
                if (isLocked) {
                    labelClass = 'locked';
                    if (isChecked) {
                        labelClass += userAnswers[currentQuestionIndex] === question.answer ? ' correct-answer' : ' wrong-answer';
                    } else if (i === question.answer) {
                        labelClass += ' correct-answer';
                    }
                } else if (isChecked) {
                    labelClass = 'selected';
                }
                
                html += `
                    <label class="${labelClass}">
                        <input type="radio" name="q${currentQuestionIndex}" value="${i}" ${isChecked ? 'checked' : ''} ${isDisabled ? 'disabled' : ''} onchange="selectAnswer(${i})">
                        ${opt}
                        ${isLocked && i === question.answer ? ' <i class="fas fa-check" style="color: var(--secondary); margin-right: 5px;"></i>' : ''}
                    </label>
                `;
            });
            
            html += `
                    </div>
                    <div id="explanation" class="explanation"></div>
                </div>
                <div class="navigation">
                    <button class="btn btn-secondary" onclick="previousQuestion()" ${currentQuestionIndex === 0 ? 'disabled' : ''}>
                        <i class="fas fa-arrow-right"></i>
                        السابق
                    </button>
                    <button class="btn btn-primary" onclick="nextQuestion()" ${currentQuestionIndex === questions.length - 1 ? 'disabled' : ''}>
                        التالي
                        <i class="fas fa-arrow-left"></i>
                    </button>
                </div>
            `;
            
            quizDiv.innerHTML = html;
            
            // تحديث شريط التقدم
            document.getElementById('progress').style.width = `${((currentQuestionIndex + 1) / questions.length) * 100}%`;
            
            // تحديث معلومات الاختبار
            document.getElementById('quiz-info').innerHTML = `السؤال ${currentQuestionIndex + 1} من ${questions.length}`;
            
            // تحديث زر وضع العلامة
            const markBtn = document.getElementById('mark-review-btn');
            if (markedQuestions.includes(currentQuestionIndex)) {
                markBtn.innerHTML = '<i class="fas fa-flag"></i> إزالة العلامة';
                markBtn.style.background = 'var(--tertiary)';
            } else {
                markBtn.innerHTML = '<i class="fas fa-flag"></i> وضع علامة للمراجعة';
                markBtn.style.background = 'var(--secondary)';
            }
            
            // عرض الشرح إذا كان المستخدم قد أجاب على السؤال
            if (userAnswers[currentQuestionIndex] !== null) {
                showExplanation();
            }
        }

        // اختيار إجابة
        function selectAnswer(answerIndex) {
            userAnswers[currentQuestionIndex] = answerIndex;
            answerLocked[currentQuestionIndex] = true; // قفل الإجابة
            showExplanation();
            loadQuiz(); // إعادة تحميل لعرض التغييرات
        }

        // عرض الشرح
        function showExplanation() {
            const question = questions[currentQuestionIndex];
            const explanationDiv = document.getElementById("explanation");
            const userAnswer = userAnswers[currentQuestionIndex];
            
            if (userAnswer !== null) {
                explanationDiv.style.display = "block";
                
                let resultHTML = "";
                
                if (userAnswer === question.answer) {
                    resultHTML = `<p class="correct"><i class="fas fa-check-circle"></i> إجابة صحيحة</p>`;
                } else {
                    resultHTML = `
                        <p class="wrong"><i class="fas fa-times-circle"></i> إجابة خاطئة — الإجابة الصحيحة: <span class="correct">${question.options[question.answer]}</span></p>
                    `;
                }
                
                // إضافة الشروح الملونة
                resultHTML += `
                    <div class="explanation-line explanation-correct"><strong>التفسير الصحيح:</strong> ${question.explanations.correct}</div>
                `;
                
                if (question.explanations.wrong1) {
                    resultHTML += `<div class="explanation-line explanation-wrong-1">${question.explanations.wrong1}</div>`;
                }
                
                if (question.explanations.wrong2) {
                    resultHTML += `<div class="explanation-line explanation-wrong-2">${question.explanations.wrong2}</div>`;
                }
                
                if (question.explanations.wrong3) {
                    resultHTML += `<div class="explanation-line explanation-wrong-3">${question.explanations.wrong3}</div>`;
                }
                
                explanationDiv.innerHTML = resultHTML;
            }
        }

        // الانتقال إلى السؤال التالي
        function nextQuestion() {
            if (currentQuestionIndex < questions.length - 1) {
                currentQuestionIndex++;
                loadQuiz();
            }
        }

        // الانتقال إلى السؤال السابق
        function previousQuestion() {
            if (currentQuestionIndex > 0) {
                currentQuestionIndex--;
                loadQuiz();
            }
        }

        // عرض الدرجات الحالية دون إنهاء الاختبار
        function showCurrentScore() {
            let totalCorrect = 0;
            userAnswers.forEach((answer, index) => {
                if (answer === questions[index].answer) {
                    totalCorrect++;
                }
            });

            const total = questions.length;
            const percentage = ((totalCorrect / total) * 100).toFixed(2);

            document.getElementById("current-score").style.display = "block";
            document.getElementById("current-correct").innerHTML = `الإجابات الصحيحة: ${totalCorrect} من ${total}`;
            document.getElementById("current-percentage").innerHTML = `النسبة المئوية الحالية: ${percentage}%`;
        }

        // حساب الدرجات النهائية
        function finishQuiz() {
            clearInterval(timerInterval);
            
            let totalCorrect = 0;
            userAnswers.forEach((answer, index) => {
                if (answer === questions[index].answer) {
                    totalCorrect++;
                }
            });

            const total = questions.length;
            const percentage = ((totalCorrect / total) * 100).toFixed(2);

            let evaluation = "";
            let evaluationIcon = "";
            if (percentage >= 90) {
                evaluation = "ممتاز";
                evaluationIcon = "🌟";
            } else if (percentage >= 80) {
                evaluation = "جيد جداً";
                evaluationIcon = "🔵";
            } else if (percentage >= 70) {
                evaluation = "جيد";
                evaluationIcon = "🟢";
            } else {
                evaluation = "يحتاج تحسين";
                evaluationIcon = "⚠️";
            }

            document.getElementById("result-box").style.display = "block";
            document.getElementById("result").innerHTML = `${evaluationIcon} النتيجة: ${totalCorrect} من ${total}`;
            document.getElementById("percentage").innerHTML = `النسبة المئوية: ${percentage}%`;
            document.getElementById("evaluation").innerHTML = `التقييم: ${evaluation}`;
            
            // إخفاء الاختبار
            document.getElementById("quiz").style.display = "none";
            document.querySelector(".controls").style.display = "none";
            document.getElementById('questions-list').style.display = 'none';
        }

        // بدء التحميل الأولي
        window.onload = function() {
            checkDarkModePreference();
            loadQuiz();
            startTimer();
        }
    </script>
</body>
</html>
