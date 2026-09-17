# Tarahan_bartar
سایت طراحی لوگو 
<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>طراحان برتر | خدمات طراحی</title>

  <meta
    name="description"
    content="طراحان برتر؛ خدمات حرفه‌ای طراحی لوگو، پوستر، منوی رستوران و طرح مهر ژلاتینی."
  >

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      font-family: Tahoma, Arial, sans-serif;
      background: #f5f6f8;
      color: #1f2937;
      line-height: 1.9;
    }

    a {
      text-decoration: none;
      color: inherit;
    }

    .container {
      width: min(1100px, 92%);
      margin: auto;
    }

    /* ================= HEADER ================= */

    header {
      background: linear-gradient(135deg, #111827, #1f2937);
      color: white;
      position: sticky;
      top: 0;
      z-index: 1000;
      box-shadow: 0 4px 20px rgba(0, 0, 0, 0.12);
    }

    .nav {
      min-height: 72px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 20px;
    }

    .logo {
      font-size: 24px;
      font-weight: 900;
      letter-spacing: -1px;
    }

    .nav-links {
      display: flex;
      gap: 8px;
      list-style: none;
    }

    .nav-links a {
      display: block;
      padding: 9px 14px;
      border-radius: 10px;
      color: #e5e7eb;
      transition: 0.2s;
    }

    .nav-links a:hover {
      background: #374151;
      color: white;
    }

    /* ================= HERO ================= */

    .hero {
      padding: 95px 0 80px;
      background:
        radial-gradient(
          circle at 15% 20%,
          rgba(99, 102, 241, 0.18),
          transparent 30%
        ),
        radial-gradient(
          circle at 85% 20%,
          rgba(14, 165, 233, 0.14),
          transparent 30%
        ),
        #111827;

      color: white;
    }

    .hero-content {
      text-align: center;
      max-width: 800px;
      margin: auto;
    }

    .badge {
      display: inline-block;
      background: #374151;
      color: #dbeafe;
      border: 1px solid #4b5563;
      padding: 5px 14px;
      border-radius: 999px;
      font-size: 13px;
      margin-bottom: 18px;
    }

    .hero h1 {
      font-size: clamp(40px, 7vw, 70px);
      line-height: 1.2;
      margin-bottom: 18px;
    }

    .hero p {
      color: #d1d5db;
      font-size: 18px;
      max-width: 680px;
      margin: 0 auto 30px;
    }

    .btn {
      display: inline-block;
      background: white;
      color: #111827;
      padding: 11px 24px;
      border-radius: 12px;
      font-weight: 800;
      transition: 0.2s;
      box-shadow: 0 8px 25px rgba(0, 0, 0, 0.15);
    }

    .btn:hover {
      transform: translateY(-3px);
    }

    /* ================= SECTIONS ================= */

    section {
      padding: 75px 0;
    }

    .section-title {
      text-align: center;
      margin-bottom: 40px;
    }

    .section-title h2 {
      font-size: 32px;
      color: #111827;
      margin-bottom: 8px;
    }

    .section-title p {
      color: #6b7280;
    }

    /* ================= SERVICES ================= */

    .services {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 20px;
    }

    .card {
      background: white;
      border: 1px solid #e5e7eb;
      border-radius: 18px;
      padding: 25px;
      box-shadow: 0 8px 30px rgba(17, 24, 39, 0.06);
      transition: 0.25s;
    }

    .card:hover {
      transform: translateY(-6px);
      box-shadow: 0 15px 35px rgba(17, 24, 39, 0.1);
    }

    .icon {
      width: 52px;
      height: 52px;
      border-radius: 14px;
      background: #111827;
      color: white;

      display: flex;
      align-items: center;
      justify-content: center;

      font-size: 23px;
      margin-bottom: 18px;
    }

    .card h3 {
      font-size: 20px;
      margin-bottom: 10px;
      color: #111827;
    }

    .card p {
      color: #6b7280;
      font-size: 14px;
      min-height: 60px;
    }

    .price {
      font-size: 22px;
      font-weight: 900;
      margin-top: 18px;
      color: #111827;
    }

    /* ================= ABOUT ================= */

    .about {
      background: white;
      border-top: 1px solid #e5e7eb;
      border-bottom: 1px solid #e5e7eb;
    }

    .about-box {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 45px;
      align-items: center;
    }

    .about h2 {
      font-size: 32px;
      margin-bottom: 15px;
      color: #111827;
    }

    .about p {
      color: #667085;
    }

    .features {
      list-style: none;
      margin-top: 10px;
    }

    .features li {
      margin: 12px 0;
      color: #374151;
      font-weight: 600;
    }

    .features li::before {
      content: "✓";
      font-weight: 900;
      margin-left: 10px;
    }

    /* ================= CONTACT ================= */

    .contact-box {
      max-width: 750px;
      margin: auto;
      text-align: center;

      background: #111827;
      color: white;

      padding: 48px 25px;
      border-radius: 24px;
      box-shadow: 0 15px 40px rgba(17, 24, 39, 0.15);
    }

    .contact-box h2 {
      font-size: 30px;
      margin-bottom: 10px;
    }

    .contact-box p {
      color: #d1d5db;
      margin-bottom: 25px;
    }

    /* ================= FOOTER ================= */

    footer {
      background: #0b1120;
      color: #9ca3af;
      text-align: center;
      padding: 25px;
      font-size: 14px;
    }

    /* ================= MOBILE ================= */

    @media (max-width: 850px) {

      .services {
        grid-template-columns: repeat(2, 1fr);
      }

      .about-box {
        grid-template-columns: 1fr;
      }
    }

    @media (max-width: 600px) {

      .nav {
        flex-direction: column;
        padding: 14px 0;
      }

      .nav-links {
        width: 100%;
        justify-content: center;
        flex-wrap: wrap;
      }

      .hero {
        padding: 65px 0;
      }

      section {
        padding: 55px 0;
      }

      .services {
        grid-template-columns: 1fr;
      }

      .hero p {
        font-size: 16px;
      }

      .card p {
        min-height: auto;
      }

      .section-title h2 {
        font-size: 28px;
      }

      .about h2 {
        font-size: 28px;
      }
    }
  </style>
</head>

<body>

  <!-- ================= HEADER ================= -->

  <header>

    <div class="container nav">

      <div class="logo">
        طراحان برتر
      </div>

      <ul class="nav-links">

        <li>
          <a href="#services">
            خدمات
          </a>
        </li>

        <li>
          <a href="#about">
            درباره ما
          </a>
        </li>

        <li>
          <a href="#contact">
            تماس
          </a>
        </li>

      </ul>

    </div>

  </header>


  <main>

    <!-- ================= HERO ================= -->

    <section class="hero">

      <div class="container hero-content">

        <span class="badge">
          استودیو خدمات طراحی
        </span>

        <h1>
          طراحان برتر
        </h1>

        <p>
          طراحی حرفه‌ای و خلاقانه برای برندها، کسب‌وکارها و افرادی
          که می‌خواهند متفاوت و حرفه‌ای دیده شوند.
        </p>

        <a
          class="btn"
          href="#services"
        >
          مشاهده خدمات
        </a>

      </div>

    </section>


    <!-- ================= SERVICES ================= -->

    <section id="services">

      <div class="container">

        <div class="section-title">

          <h2>
            خدمات ما
          </h2>

          <p>
            خدمات طراحی با ظاهر حرفه‌ای و مناسب استفاده دیجیتال و چاپ
          </p>

        </div>


        <div class="services">


          <!-- LOGO -->

          <article class="card">

            <div class="icon">
              ✦
            </div>

            <h3>
              طراحی لوگو
            </h3>

            <p>
              طراحی لوگوی اختصاصی و حرفه‌ای متناسب با هویت کسب‌وکار شما.
            </p>

            <div class="price">
              ۲۰۰ تومان
            </div>

          </article>


          <!-- POSTER -->

          <article class="card">

            <div class="icon">
              ▣
            </div>

            <h3>
              طراحی پوستر
            </h3>

            <p>
              طراحی پوستر تبلیغاتی و معرفی خدمات با ظاهر جذاب و مدرن.
            </p>

            <div class="price">
              ۲۵۰ تومان
            </div>

          </article>


          <!-- MENU -->

          <article class="card">

            <div class="icon">
              ☰
            </div>

            <h3>
              طراحی منوی رستوران
            </h3>

            <p>
              طراحی منوی شیک و خوانا برای کافه‌ها، رستوران‌ها و فست‌فودها.
            </p>

            <div class="price">
              ۳۰۰ تومان
            </div>

          </article>


          <!-- STAMP -->

          <article class="card">

            <div class="icon">
              ◎
            </div>

            <h3>
              طراحی طرح مهر ژلاتینی
            </h3>

            <p>
              آماده‌سازی طرح مناسب ساخت مهر ژلاتینی و استفاده چاپی.
            </p>

            <div class="price">
              ۱۰۰ تومان
            </div>

          </article>


        </div>

      </div>

    </section>


    <!-- ================= ABOUT ================= -->

    <section id="about" class="about">

      <div class="container about-box">


        <div>

          <h2>
            چرا طراحان برتر؟
          </h2>

          <p>
            هدف ما ارائه طرح‌هایی است که هم زیبا و حرفه‌ای باشند
            و هم بتوانید در دنیای واقعی و فضای دیجیتال از آن‌ها
            استفاده کنید.
          </p>

        </div>


        <ul class="features">

          <li>
            طراحی اختصاصی
          </li>

          <li>
            ظاهر مدرن و حرفه‌ای
          </li>

          <li>
            مناسب چاپ و استفاده دیجیتال
          </li>

          <li>
            توجه به جزئیات
          </li>

        </ul>


      </div>

    </section>


    <!-- ================= CONTACT ================= -->

    <section id="contact">

      <div class="container">

        <div class="contact-box">

          <h2>
            برای سفارش طراحی
          </h2>

          <p>
            برای سفارش هر یک از خدمات طراحی،
            با طراحان برتر در ارتباط باشید و طرح مورد نیاز
            خود را سفارش دهید.
          </p>

          <a
            class="btn"
            href="#services"
          >
            مشاهده خدمات و قیمت‌ها
          </a>

        </div>

      </div>

    </section>

  </main>


  <!-- ================= FOOTER ================= -->

  <footer>

    © ۲۰۲۶ طراحان برتر — تمامی حقوق محفوظ است.

  </footer>


</body>
</html>
