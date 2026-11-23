<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>منصة Mr. Mahrous | للغة العربية</title>
    <style>
        :root {
            --primary-color: #1e3a8a;
            --accent-color: #3b82f6;
            --text-color: #333;
            --bg-light: #f8fafc;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: var(--bg-light);
            color: var(--text-color);
            scroll-behavior: smooth;
        }

        /* القائمة العلوية */
        .navbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 5%;
            background: white;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            position: sticky;
            top: 0;
            z-index: 1000;
            transition: background 0.3s ease;
        }

        .logo {
            font-size: 1.5rem;
            font-weight: bold;
            color: var(--primary-color);
        }

        .nav-links {
            list-style: none;
            display: flex;
            gap: 20px;
        }

        .nav-links a {
            text-decoration: none;
            color: var(--text-color);
            font-weight: 500;
            transition: color 0.3s;
        }

        .nav-links a:hover {
            color: var(--accent-color);
        }

        .login-btn, button {
            background: var(--primary-color);
            color: white;
            border: none;
            padding: 10px 20px;
            border-radius: 5px;
            cursor: pointer;
            font-family: inherit;
            transition: background 0.3s;
        }

        .login-btn:hover, button:hover {
            background: var(--accent-color);
        }

        /* قسم الترحيب */
        .hero-section {
            height: 60vh;
            background: linear-gradient(rgba(30, 58, 138, 0.8), rgba(30, 58, 138, 0.8)), 
                        url('https://images.unsplash.com/photo-1455390582262-044cdead277a?auto=format&fit=crop&w=1350&q=80');
            background-size: cover;
            background-position: center;
            display: flex;
            justify-content: center;
            align-items: center;
            color: white;
            text-align: center;
            padding: 0 20px;
        }

        .hero-content h1 {
            font-size: 2.5rem;
            margin-bottom: 15px;
        }

        .hero-content p {
            font-size: 1.2rem;
            margin-bottom: 20px;
        }

        .cta-button {
            background: var(--accent-color);
            color: white;
            padding: 12px 30px;
            border-radius: 25px;
            text-decoration: none;
            display: inline-block;
            font-weight: bold;
            transition: background 0.3s, transform 0.2s;
        }

        .cta-button:hover {
            background: #2563eb;
            transform: scale(1.05);
        }

        /* الكروت */
        .section { 
            padding: 50px 5%; 
        }
        
        .section-title { 
            text-align: center; 
            margin-bottom: 40px; 
            font-size: 2rem;
            color: var(--primary-color);
        }

        .cards-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 25px;
        }

        .card {
            background: white;
            padding: 30px 20px;
            border-radius: 15px;
            text-align: center;
            transition: transform 0.3s, box-shadow 0.3s;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
        }

        .card:hover { 
            transform: translateY(-10px); 
            box-shadow: 0 10px 20px rgba(0,0,0,0.1);
        }

        .card-img { 
            font-size: 50px; 
            margin-bottom: 15px; 
        }

        .card h3 {
            margin-bottom: 10px;
            color: var(--primary-color);
        }

        .card p {
            color: #666;
            margin-bottom: 20px;
        }
    </style>
</head>
<body>

    <!-- القائمة العلوية -->
    <nav class="navbar">
        <div class="logo">Mr. Mahrous 🖋️</div>
        <ul class="nav-links">
            <li><a href="#home">الرئيسية</a></li>
            <li><a href="#courses">المحاضرات</a></li>
            <li><a href="#books">المكتبة</a></li>
            <li><a href="#contact">تواصل معنا</a></li>
        </ul>
        <button class="login-btn" onclick="alert('صفحة تسجيل الدخول قيد التطوير')">تسجيل دخول</button>
    </nav>

    <!-- القسم الرئيسي -->
    <header id="home" class="hero-section">
        <div class="hero-content">
            <h1>لغتنا العربية.. هوية وإبداع</h1>
            <p>تعلم اللغة العربية بأسلوب حديث ومبسط مع المستر محروس.</p>
            <a href="#courses" class="cta-button">ابدأ التعلم الآن</a>
        </div>
    </header>

    <!-- قسم المحاضرات -->
    <section id="courses" class="section">
        <h2 class="section-title">المحاضرات المتاحة</h2>
        <div class="cards-container">
            <div class="card">
                <div class="card-img">🎬</div>
                <h3>شرح درس النحو</h3>
                <p>الصف الأول الثانوي - الترم الثاني</p>
                <button onclick="showAlert()">مشاهدة الآن</button>
            </div>
            <div class="card">
                <div class="card-img">📖</div>
                <h3>بلاغة العصر العباسي</h3>
                <p>أساسيات البلاغة لطلاب الثانوي</p>
                <button onclick="showAlert()">مشاهدة الآن</button>
            </div>
            <div class="card">
                <div class="card-img">📝</div>
                <h3>بنك الأسئلة الشامل</h3>
                <p>اختبارات تفاعلية لتقييم مستواك</p>
                <button onclick="window.location.href='#home'">ابدأ الاختبار</button>
            </div>
        </div>
    </section>

    <!-- كود التفاعل (JavaScript) -->
    <script>
        function showAlert() {
            alert("سيتم فتح المحاضرة قريباً.. تأكد من تسجيل دخولك أولاً!");
        }

        // إضافة تأثير ديناميكي عند التمرير على شريط التنقل
        window.addEventListener('scroll', () => {
            const nav = document.querySelector('.navbar');
            if (window.scrollY > 50) {
                nav.style.background = '#f1f5f9';
            } else {
                nav.style.background = 'white';
            }
        });
    </script>
</body>
</html>
