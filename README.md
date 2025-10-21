`html
<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>مهدی آراسته - کارگردان و بازیگر تئاتر</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background: linear-gradient(135deg, #1a1a1a 0%, #2d2d2d 100%);
            color: #fff;
            line-height: 1.6;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* هدر و نویگیشن */
        header {
            background: rgba(0, 0, 0, 0.9);
            padding: 1rem 0;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            backdrop-filter: blur(10px);
        }

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 1.8rem;
            font-weight: bold;
            color: #e74c3c;
        }

        .nav-links {
            display: flex;
            list-style: none;
            gap: 2rem;
        }

        .nav-links a {
            color: #fff;
            text-decoration: none;
            transition: color 0.3s;
        }

        .nav-links a:hover {
            color: #e74c3c;
        }

        /* هیرو سکشن */
        .hero {
            height: 100vh;
            display: flex;
            align-items: center;
            background: linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.7)), url('pattern.png');
            text-align: center;
        }

        .hero-content h1 {
            font-size: 3.5rem;
            margin-bottom: 1rem;
            background: linear-gradient(45deg, #e74c3c, #f39c12);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .hero-content p {
            font-size: 1.3rem;
            margin-bottom: 2rem;
            color: #ccc;
        }

        .btn {
            display: inline-block;
            padding: 12px 30px;
            background: #e74c3c;
            color: white;
            text-decoration: none;
            border-radius: 5px;
            transition: background 0.3s;
        }

        .btn:hover {
            background: #c0392b;
        }

        /* گالری */
        .gallery {
            padding: 5rem 0;
        }

        .section-title {
            text-align: center;
            font-size: 2.5rem;
            margin-bottom: 3rem;
            color: #e74c3c;
        }

        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }

        .project-card {
            background: rgba(255, 255, 255, 0.1);
            border-radius: 10px;
            overflow: hidden;
            transition: transform 0.3s;
        }





        .project-card:hover {
            transform: translateY(-10px);
        }

        .project-img {
            width: 100%;
            height: 250px;
            object-fit: cover;
        }

        .project-info {
            padding: 1.5rem;
        }

        .project-info h3 {
            color: #f39c12;
            margin-bottom: 0.5rem;
        }

        /* بخش تماس */
        .contact {
            padding: 5rem 0;
            background: rgba(0, 0, 0, 0.5);
        }

        .contact-info {
            text-align: center;
            font-size: 1.2rem;
        }

        .email {
            color: #e74c3c;
            font-size: 1.4rem;
            margin: 1rem 0;
        }

        /* فوتور */
        footer {
            background: #000;
            padding: 2rem 0;
            text-align: center;
            color: #666;
        }

        /* رسپانسیو */
        @media (max-width: 768px) {
            .nav-links {
                display: none;
            }
            
            .hero-content h1 {
                font-size: 2.5rem;
            }
            
            .projects-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <header>
        <nav class="container">
            <div class="logo">مهدی آراسته</div>
            <ul class="nav-links">
                <li><a href="#home">خانه</a></li>
                <li><a href="#bio">بیوگرافی</a></li>
                <li><a href="#gallery">آثار</a></li>
                <li><a href="#contact">تماس</a></li>
            </ul>
        </nav>
    </header>

    <section id="home" class="hero">
        <div class="container hero-content">
            <h1>مهدی آراسته</h1>
            <p>کارگردان، بازیگر و نویسنده تئاتر، سینما و موسیقی</p>
            <p>کارگردانی ۲۱ اثر ماندگار در عرصه تئاتر</p>
            <a href="#gallery" class="btn">مشاهده آثار</a>
        </div>
    </section>

    <section id="gallery" class="gallery">
        <div class="container">
            <h2 class="section-title">گالری آثار</h2>
            <div class="projects-grid">
                <!-- کارت‌های آثار به صورت داینامیک اضافه خواهند شد -->
                <div class="project-card">
                    <img src="poster1.jpg" alt="مرگ یزدگرد" class="project-img">
                    <div class="project-info">
                        <h3>مرگ یزدگرد</h3>
                        <p>نویسنده: بهرام بیضایی</p>
                        <p>زمان: ۱۲-۱۳ خرداد ۱۴۰۳</p>
                    </div>
                </div>
                <!-- بقیه کارت‌ها... -->
            </div>
        </div>
    </section>

    <section id="contact" class="contact">
        <div class="container">
            <h2 class="section-title">تماس با من</h2>
            <div class="contact-info">
                <p>برای همکاری و اطلاعات بیشتر:</p>
                <div class="email">mahdi.arasteh82@gmail.com</div>
                <p>کارگردان، بازیگر، نویسنده و نمایشنامه‌نویس</p>
            </div>
        </div>
    </section>

    <footer>
        <div class="container">
            <p>© ۲۰۲۴ - کلیه حقوق محفوظ است</p>
        </div>
    </footer>

    <script>
        // اسکرول نرم برای لینک‌ها
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });
    </script>
</body>
</html>
`

