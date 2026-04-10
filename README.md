# zaddysslatty.github.io
<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Pulsoft — Пульс твоего пространства</title>
<meta name="description" content="Pulsoft — B2B-компания в сфере experience design. Превращаем готовые объекты в живые пространства через исследования, сценарии, навигацию и активации.">
<meta name="keywords" content="experience design, пространственный консалтинг, активация пространств, placemaking, урбанистика, дизайн среды, поведенческая архитектура">
<link href="https://fonts.googleapis.com/css2?family=Manrope:wght@300;400;500;600;700;800&family=Unbounded:wght@500;700;900&display=swap" rel="stylesheet">
<style>
  :root{
    --burgundy:#4a0d12;
    --burgundy-deep:#2e0609;
    --cream:#f7f3ee;
    --beige:#e8d5b7;
    --gold:#c9a96e;
    --white:#ffffff;
    --gray:#6b6b6b;
    --gray-light:#eeeae4;
  }
  *{margin:0;padding:0;box-sizing:border-box}
  html{scroll-behavior:smooth}
  body{
    font-family:'Manrope',sans-serif;
    color:#1a1a1a;
    background:var(--cream);
    line-height:1.55;
    -webkit-font-smoothing:antialiased;
  }
  h1,h2,h3,h4{font-family:'Unbounded','Manrope',sans-serif;font-weight:700;letter-spacing:-0.01em;line-height:1.15;overflow-wrap:break-word;word-wrap:break-word;hyphens:auto}
  .container{max-width:1200px;margin:0 auto;padding:0 28px}

  /* NAV */
  nav{
    position:fixed;top:0;left:0;right:0;z-index:100;
    padding:18px 0;background:rgba(247,243,238,.85);
    backdrop-filter:blur(12px);
    border-bottom:1px solid rgba(0,0,0,.05);
  }
  nav .container{display:flex;align-items:center;justify-content:space-between}
  .logo{display:flex;align-items:center;gap:12px;text-decoration:none;color:var(--burgundy)}
  .logo svg{width:38px;height:38px}
  .logo span{font-family:'Unbounded',sans-serif;font-weight:900;font-size:20px;letter-spacing:2px}
  .nav-links{display:flex;gap:36px}
  .nav-links a{color:#1a1a1a;text-decoration:none;font-size:15px;font-weight:500;transition:color .2s}
  .nav-links a:hover{color:var(--burgundy)}
  .nav-cta{
    background:var(--burgundy);color:#fff;padding:12px 24px;
    border-radius:100px;text-decoration:none;font-size:14px;font-weight:600;
    transition:all .3s;
  }
  .nav-cta:hover{background:var(--burgundy-deep);transform:translateY(-1px)}

  /* HERO */
  .hero{
    min-height:100vh;padding:160px 0 80px;position:relative;overflow:hidden;
    background:radial-gradient(circle at 80% 20%, rgba(74,13,18,.08), transparent 60%), var(--cream);
  }
  .hero .container{position:relative;z-index:2}
  .hero-eyebrow{
    display:inline-flex;align-items:center;gap:10px;
    padding:8px 18px;border:1px solid rgba(74,13,18,.2);border-radius:100px;
    font-size:13px;color:var(--burgundy);font-weight:600;margin-bottom:28px;
    text-transform:uppercase;letter-spacing:1.5px;
  }
  .pulse-dot{width:8px;height:8px;background:var(--burgundy);border-radius:50%;animation:pulse 2s infinite}
  @keyframes pulse{
    0%{box-shadow:0 0 0 0 rgba(74,13,18,.5)}
    70%{box-shadow:0 0 0 14px rgba(74,13,18,0)}
    100%{box-shadow:0 0 0 0 rgba(74,13,18,0)}
  }
  .hero h1{
    font-size:clamp(40px,6.5vw,88px);
    color:var(--burgundy);
    margin-bottom:28px;max-width:900px;
  }
  .hero h1 em{font-style:normal;color:var(--gold)}
  .hero-sub{
    font-size:clamp(17px,1.6vw,22px);
    max-width:640px;color:#3a3a3a;margin-bottom:44px;font-weight:400;
  }
  .hero-quote{
    font-family:'Unbounded',sans-serif;font-size:15px;
    color:var(--burgundy);font-weight:500;margin-bottom:44px;
    padding-left:18px;border-left:3px solid var(--gold);
    max-width:520px;
  }
  .btn-group{display:flex;gap:16px;flex-wrap:wrap}
  .btn-primary{
    background:var(--burgundy);color:#fff;padding:18px 38px;
    border-radius:100px;text-decoration:none;font-weight:600;font-size:16px;
    transition:all .3s;display:inline-flex;align-items:center;gap:10px;
    box-shadow:0 10px 30px rgba(74,13,18,.25);
  }
  .btn-primary:hover{background:var(--burgundy-deep);transform:translateY(-2px);box-shadow:0 14px 40px rgba(74,13,18,.35)}
  .btn-secondary{
    background:transparent;color:var(--burgundy);padding:18px 38px;
    border:1.5px solid var(--burgundy);border-radius:100px;text-decoration:none;
    font-weight:600;font-size:16px;transition:all .3s;
  }
  .btn-secondary:hover{background:var(--burgundy);color:#fff}
  .hero-visual{
    position:absolute;right:-100px;top:50%;transform:translateY(-50%);
    width:600px;height:600px;opacity:.12;pointer-events:none;
  }

  /* SECTIONS */
  section{padding:120px 0;position:relative}
  .section-label{
    display:inline-block;font-size:12px;font-weight:700;letter-spacing:2px;
    text-transform:uppercase;color:var(--burgundy);margin-bottom:20px;
  }
  .section-title{
    font-size:clamp(34px,4.5vw,58px);color:var(--burgundy);
    max-width:800px;margin-bottom:24px;
  }
  .section-intro{font-size:18px;color:#3a3a3a;max-width:680px;margin-bottom:60px}

  /* PROBLEM */
  .problem{background:var(--burgundy);color:#fff}
  .problem .section-label{color:var(--gold)}
  .problem .section-title{color:#fff}
  .problem-grid{display:grid;grid-template-columns:1fr 1fr;gap:40px;margin-top:40px}
  .problem-card{
    padding:48px 40px;border:1px solid rgba(255,255,255,.15);border-radius:20px;
    background:rgba(255,255,255,.03);transition:all .3s;
  }
  .problem-card:hover{background:rgba(255,255,255,.06);transform:translateY(-4px)}
  .problem-card .num{
    font-family:'Unbounded',sans-serif;font-size:60px;font-weight:900;
    color:var(--gold);opacity:.5;line-height:1;margin-bottom:20px;
  }
  .problem-card h3{font-size:24px;margin-bottom:14px;color:#fff}
  .problem-card p{color:rgba(255,255,255,.75);font-size:16px}

  /* SOLUTION */
  .solution{background:var(--cream)}
  .solution-grid{display:grid;grid-template-columns:1.2fr 1fr;gap:80px;align-items:center}
  .solution-visual{
    aspect-ratio:1;background:var(--burgundy);border-radius:24px;
    display:flex;align-items:center;justify-content:center;position:relative;overflow:hidden;
  }
  .solution-visual svg{width:70%;height:70%;opacity:.9}

  /* SERVICES */
  .services{background:var(--white)}
  .services-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(260px,1fr));gap:24px}
  .service-card{
    padding:40px 32px;background:var(--cream);border-radius:20px;
    transition:all .35s;border:1px solid transparent;position:relative;overflow:hidden;
  }
  .service-card:hover{
    background:var(--burgundy);color:#fff;transform:translateY(-6px);
    box-shadow:0 20px 50px rgba(74,13,18,.2);
  }
  .service-card:hover h3,.service-card:hover p{color:#fff}
  .service-card:hover .service-icon{background:rgba(255,255,255,.15);color:#fff}
  .service-icon{
    width:56px;height:56px;border-radius:14px;background:var(--burgundy);
    color:#fff;display:flex;align-items:center;justify-content:center;
    margin-bottom:24px;font-size:24px;font-weight:900;transition:all .3s;
    font-family:'Unbounded',sans-serif;
  }
  .service-card h3{font-size:19px;margin-bottom:12px;color:var(--burgundy);transition:color .3s;line-height:1.25}
  .service-card p{font-size:15px;color:#555;transition:color .3s}

  /* AUDIENCE */
  .audience{background:var(--cream)}
  .audience-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(270px,1fr));gap:22px}
  .audience-card{
    padding:40px 32px;background:#fff;border-radius:20px;
    border:1px solid var(--gray-light);transition:all .3s;
  }
  .audience-card:hover{border-color:var(--burgundy);transform:translateY(-4px);box-shadow:0 16px 40px rgba(0,0,0,.06)}
  .audience-card .tag{
    display:inline-block;padding:6px 14px;background:var(--burgundy);color:#fff;
    border-radius:100px;font-size:12px;font-weight:600;margin-bottom:20px;letter-spacing:.5px;
  }
  .audience-card h3{font-size:22px;color:var(--burgundy);margin-bottom:12px}
  .audience-card .pain{font-size:14px;color:var(--gray);margin-bottom:16px;font-style:italic}
  .audience-card .solution-txt{font-size:15px;color:#1a1a1a}

  /* WHY */
  .why{background:var(--white)}
  .why-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:40px;margin-top:20px}
  .why-item{padding-top:32px;border-top:2px solid var(--burgundy)}
  .why-item .num{
    font-family:'Unbounded',sans-serif;font-size:16px;font-weight:900;
    color:var(--gold);margin-bottom:14px;
  }
  .why-item h3{font-size:22px;color:var(--burgundy);margin-bottom:14px}
  .why-item p{font-size:15px;color:#444}

  /* MODEL */
  .model{background:var(--burgundy-deep);color:#fff}
  .model .section-label{color:var(--gold)}
  .model .section-title{color:#fff}
  .model-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(240px,1fr));gap:20px;margin-top:40px}
  .model-card{
    padding:36px 28px;background:rgba(255,255,255,.04);border-radius:18px;
    border:1px solid rgba(255,255,255,.1);transition:all .3s;
  }
  .model-card:hover{background:rgba(255,255,255,.08);border-color:var(--gold)}
  .model-card .icon{
    font-family:'Unbounded',sans-serif;font-size:14px;color:var(--gold);
    font-weight:700;margin-bottom:14px;display:block;
  }
  .model-card h3{font-size:19px;margin-bottom:10px;color:#fff}
  .model-card p{font-size:14px;color:rgba(255,255,255,.7)}

  /* MARKET */
  .market{background:var(--cream);text-align:center}
  .market-stat{
    font-family:'Unbounded',sans-serif;font-size:clamp(54px,9vw,130px);
    color:var(--burgundy);font-weight:900;line-height:1;margin:40px 0 20px;
    white-space:nowrap;
  }
  .market-stat em{font-style:normal;color:var(--gold)}
  .market-caption{font-size:18px;color:#444;max-width:560px;margin:0 auto 30px}
  .market-trend{
    display:inline-block;padding:14px 28px;background:#fff;
    border-radius:100px;font-size:15px;color:var(--burgundy);font-weight:600;
    border:1px solid var(--gray-light);
  }

  /* TEAM */
  .team{background:var(--white)}
  .team-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(200px,1fr));gap:20px}
  .team-card{
    padding:32px 24px;background:var(--cream);border-radius:18px;text-align:center;
    transition:all .3s;
  }
  .team-card:hover{background:var(--burgundy);color:#fff;transform:translateY(-4px)}
  .team-card:hover h4{color:#fff}
  .team-card:hover p{color:rgba(255,255,255,.75)}
  .team-avatar{
    width:64px;height:64px;border-radius:50%;background:var(--burgundy);
    margin:0 auto 16px;display:flex;align-items:center;justify-content:center;
    color:#fff;font-family:'Unbounded',sans-serif;font-weight:900;font-size:22px;
  }
  .team-card:hover .team-avatar{background:var(--gold);color:var(--burgundy-deep)}
  .team-card h4{font-size:16px;color:var(--burgundy);margin-bottom:6px;transition:color .3s;line-height:1.25}
  .team-card p{font-size:13px;color:var(--gray);transition:color .3s}

  /* CTA */
  .cta-section{
    background:linear-gradient(135deg,var(--burgundy) 0%,var(--burgundy-deep) 100%);
    color:#fff;text-align:center;
  }
  .cta-section .section-title{color:#fff;margin-left:auto;margin-right:auto}
  .cta-form{
    max-width:680px;margin:50px auto 0;display:grid;grid-template-columns:1fr 1fr;gap:16px;
  }
  .cta-form input,.cta-form textarea{
    padding:18px 22px;background:rgba(255,255,255,.08);border:1px solid rgba(255,255,255,.15);
    border-radius:14px;color:#fff;font-size:15px;font-family:inherit;
    transition:all .3s;
  }
  .cta-form input:focus,.cta-form textarea:focus{
    outline:none;border-color:var(--gold);background:rgba(255,255,255,.12);
  }
  .cta-form input::placeholder,.cta-form textarea::placeholder{color:rgba(255,255,255,.5)}
  .cta-form textarea{grid-column:1/-1;min-height:110px;resize:vertical}
  .cta-form button{
    grid-column:1/-1;padding:20px;background:var(--gold);color:var(--burgundy-deep);
    border:none;border-radius:100px;font-size:16px;font-weight:700;font-family:inherit;
    cursor:pointer;transition:all .3s;letter-spacing:.5px;
  }
  .cta-form button:hover{background:#e0bd7a;transform:translateY(-2px)}

  /* FOOTER */
  footer{background:var(--burgundy-deep);color:rgba(255,255,255,.7);padding:80px 0 40px}
  .footer-grid{display:grid;grid-template-columns:2fr 1fr 1fr;gap:60px;margin-bottom:60px}
  .footer-brand .logo{color:#fff;margin-bottom:20px}
  .footer-brand p{font-size:15px;max-width:320px;line-height:1.7}
  .footer-col h4{color:#fff;font-size:15px;margin-bottom:20px;font-family:'Manrope',sans-serif;font-weight:700}
  .footer-col a{display:block;color:rgba(255,255,255,.6);text-decoration:none;margin-bottom:12px;font-size:14px;transition:color .2s}
  .footer-col a:hover{color:var(--gold)}
  .footer-bottom{
    border-top:1px solid rgba(255,255,255,.1);padding-top:30px;
    display:flex;justify-content:space-between;font-size:13px;flex-wrap:wrap;gap:16px;
  }

  /* Reveal animation */
  .reveal{opacity:0;transform:translateY(30px);transition:all .8s ease}
  .reveal.visible{opacity:1;transform:translateY(0)}

  /* Responsive */
  @media(max-width:900px){
    .nav-links{display:none}
    .problem-grid,.solution-grid,.why-grid,.footer-grid{grid-template-columns:1fr;gap:30px}
    .cta-form{grid-template-columns:1fr}
    section{padding:80px 0}
    .hero{padding:140px 0 60px}
    .hero-visual{display:none}
  }
</style>
</head>
<body>

<!-- SVG Logo definition -->
<svg width="0" height="0" style="position:absolute">
  <defs>
    <symbol id="logo-mark" viewBox="0 0 520 320">
      <g stroke="currentColor" stroke-width="10" fill="none">
        <rect x="5" y="5" width="510" height="310"/>
        <line x1="325" y1="5" x2="325" y2="315"/>
        <line x1="325" y1="205" x2="515" y2="205"/>
        <line x1="405" y1="205" x2="405" y2="315"/>
        <line x1="325" y1="245" x2="405" y2="245"/>
        <line x1="365" y1="205" x2="365" y2="245"/>
        <path d="M 5 315 A 310 310 0 0 1 325 5 A 200 200 0 0 1 515 205 A 110 110 0 0 1 405 315 A 80 80 0 0 1 325 245 A 40 40 0 0 1 365 205"/>
      </g>
    </symbol>
  </defs>
</svg>

<nav>
  <div class="container">
    <a href="#" class="logo">
      <svg viewBox="0 0 520 320"><use href="#logo-mark"/></svg>
      <span>PULSOFT</span>
    </a>
    <div class="nav-links">
      <a href="#services">Услуги</a>
      <a href="#audience">Клиенты</a>
      <a href="#why">Почему мы</a>
      <a href="#team">Команда</a>
    </div>
    <a href="#contact" class="nav-cta">Обсудить проект</a>
  </div>
</nav>

<!-- HERO -->
<section class="hero">
  <svg class="hero-visual" viewBox="0 0 520 320"><use href="#logo-mark"/></svg>
  <div class="container">
    <div class="hero-eyebrow reveal"><span class="pulse-dot"></span> EXPERIENCE DESIGN · B2B</div>
    <h1 class="reveal">Pulsoft —<br>пульс твоего <em>пространства</em>.</h1>
    <p class="hero-sub reveal">Превращаем готовые объекты в любимые и живые места. Без капитальных ремонтов и больших вложений.</p>
    <p class="hero-quote reveal">Мы не проектируем стены. Мы проектируем жизнь внутри них.</p>
    <div class="btn-group reveal">
      <a href="#contact" class="btn-primary">Оживить пространство →</a>
      <a href="#services" class="btn-secondary">Что мы делаем</a>
    </div>
  </div>
</section>

<!-- PROBLEM -->
<section class="problem">
  <div class="container">
    <span class="section-label reveal">Проблема</span>
    <h2 class="section-title reveal">Красивое здание ещё не значит живое место.</h2>
    <div class="problem-grid">
      <div class="problem-card reveal">
        <div class="num">01</div>
        <h3>Пространство, которым не пользуются — это деньги на ветер.</h3>
        <p>Вложения в архитектуру и отделку не возвращаются, если среда не вовлекает людей в ежедневную жизнь.</p>
      </div>
      <div class="problem-card reveal">
        <div class="num">02</div>
        <h3>Объект построен — но место «мёртвое».</h3>
        <p>Нет вовлечённости, нет активности, нет сообщества. Жители, сотрудники и гости проходят мимо.</p>
      </div>
    </div>
  </div>
</section>

<!-- SOLUTION -->
<section class="solution">
  <div class="container">
    <div class="solution-grid">
      <div class="reveal">
        <span class="section-label">Решение</span>
        <h2 class="section-title">Мы мягко перенастраиваем среду.</h2>
        <p class="section-intro">Pulsoft — B2B-компания в сфере пространственного опыта. Мы исследуем поведение людей в готовых пространствах и проектируем сценарии жизни, навигацию, зонирование, активации и события. Клиент платит за то, чтобы объект не просто выглядел красиво, а реально использовался и работал.</p>
        <a href="#services" class="btn-primary">Посмотреть услуги →</a>
      </div>
      <div class="solution-visual reveal">
        <svg viewBox="0 0 520 320" style="color:var(--cream)"><use href="#logo-mark"/></svg>
      </div>
    </div>
  </div>
</section>

<!-- SERVICES -->
<section class="services" id="services">
  <div class="container">
    <span class="section-label reveal">Что мы делаем</span>
    <h2 class="section-title reveal">Пять направлений, которые оживляют любое пространство.</h2>
    <div class="services-grid">
      <div class="service-card reveal">
        <div class="service-icon">01</div>
        <h3>Исследование среды</h3>
        <p>Полевые наблюдения, глубинные интервью, карта потоков и сценариев поведения.</p>
      </div>
      <div class="service-card reveal">
        <div class="service-icon">02</div>
        <h3>Сценарное проектирование</h3>
        <p>Карты активности для студентов, семей, фрилансеров, команд и гостей.</p>
      </div>
      <div class="service-card reveal">
        <div class="service-icon">03</div>
        <h3>Пространственные решения</h3>
        <p>Зонирование, навигация, графика, мебель и микроархитектура.</p>
      </div>
      <div class="service-card reveal">
        <div class="service-icon">04</div>
        <h3>Сценарии событий</h3>
        <p>Гайды и форматы мероприятий, клубов, воркшопов и регулярных активаций.</p>
      </div>
      <div class="service-card reveal">
        <div class="service-icon">05</div>
        <h3>Цифровая аналитика</h3>
        <p>Дашборды для управления пространством на основе данных и поведения пользователей.</p>
      </div>
    </div>
  </div>
</section>

<!-- AUDIENCE -->
<section class="audience" id="audience">
  <div class="container">
    <span class="section-label reveal">Для кого мы работаем</span>
    <h2 class="section-title reveal">Мы работаем с теми, у кого объект уже стоит.</h2>
    <div class="audience-grid">
      <div class="audience-card reveal">
        <span class="tag">Девелоперы</span>
        <h3>ЖК, МФЦ, коворкинги</h3>
        <p class="pain">«Место не ожило, жители не общаются»</p>
        <p class="solution-txt">Сценарии жизни, навигация и дизайн, превращающие двор и лобби в точки притяжения.</p>
      </div>
      <div class="audience-card reveal">
        <span class="tag">Образование</span>
        <h3>Вузы и школы</h3>
        <p class="pain">«Кампус мёртвый после пар»</p>
        <p class="solution-txt">Хаб-проекты, событийная программа и пространственные решения для студенческой жизни.</p>
      </div>
      <div class="audience-card reveal">
        <span class="tag">Город</span>
        <h3>Муниципалитеты и парки</h3>
        <p class="pain">«Пространство не используется»</p>
        <p class="solution-txt">Активация общественных зон, навигация и микроархитектура для горожан.</p>
      </div>
      <div class="audience-card reveal">
        <span class="tag">Бизнес</span>
        <h3>Бизнес-центры</h3>
        <p class="pain">«У сотрудников нет своего места»</p>
        <p class="solution-txt">Workplace-сценарии и зонирование, где хочется оставаться и работать.</p>
      </div>
    </div>
  </div>
</section>

<!-- WHY -->
<section class="why" id="why">
  <div class="container">
    <span class="section-label reveal">Почему Pulsoft</span>
    <h2 class="section-title reveal">Архитектура поведения, дизайн опыта и урбанистика в одном флаконе.</h2>
    <div class="why-grid">
      <div class="why-item reveal">
        <div class="num">01 / ФОКУС</div>
        <h3>Не конкурируем с архитекторами</h3>
        <p>Мы работаем с готовым объектом: там, где стройка уже закончилась, а жизнь ещё не началась.</p>
      </div>
      <div class="why-item reveal">
        <div class="num">02 / ЛЮДИ</div>
        <h3>Фокус на поведении</h3>
        <p>Главный материал для нас — не бетон, а сценарии, привычки и ритуалы пользователей пространства.</p>
      </div>
      <div class="why-item reveal">
        <div class="num">03 / ДАННЫЕ</div>
        <h3>Data-driven подход</h3>
        <p>Решения принимаются на основе метрик, наблюдений и дашбордов, а не интуиции.</p>
      </div>
    </div>
  </div>
</section>

<!-- MODEL -->
<section class="model">
  <div class="container">
    <span class="section-label reveal">Форматы сотрудничества</span>
    <h2 class="section-title reveal">Четыре способа работать с нами.</h2>
    <div class="model-grid">
      <div class="model-card reveal">
        <span class="icon">01</span>
        <h3>Проектный контракт</h3>
        <p>Разовые проекты с чёткими сроками и результатом.</p>
      </div>
      <div class="model-card reveal">
        <span class="icon">02</span>
        <h3>Абонентское сопровождение</h3>
        <p>Долгосрочное партнёрство и постоянная оптимизация среды.</p>
      </div>
      <div class="model-card reveal">
        <span class="icon">03</span>
        <h3>Готовые пакеты</h3>
        <p>Быстрый старт с типовыми решениями под задачи сегмента.</p>
      </div>
      <div class="model-card reveal">
        <span class="icon">04</span>
        <h3>Лицензия на гайды</h3>
        <p>Методики и playbook для сетей, франшиз и крупных операторов.</p>
      </div>
    </div>
  </div>
</section>

<!-- MARKET -->
<section class="market">
  <div class="container">
    <span class="section-label reveal">Рынок и тренды</span>
    <h2 class="section-title reveal" style="margin-left:auto;margin-right:auto">Мир переходит от красивого объекта к живой среде.</h2>
    <div class="market-stat reveal">₽28<em> трлн</em></div>
    <p class="market-caption reveal">Объём глобального рынка архитектурных и пространственных услуг к 2030 году.</p>
    <div class="market-trend reveal">↗ Рост спроса на experience design и data-driven управление пространством</div>
  </div>
</section>

<!-- TEAM -->
<section class="team" id="team">
  <div class="container">
    <span class="section-label reveal">Команда</span>
    <h2 class="section-title reveal">Междисциплинарный состав под каждый проект.</h2>
    <div class="team-grid">
      <div class="team-card reveal">
        <div class="team-avatar">UX</div>
        <h4>UX-исследователь</h4>
        <p>Наблюдения и интервью</p>
      </div>
      <div class="team-card reveal">
        <div class="team-avatar">SC</div>
        <h4>Сценарный дизайнер</h4>
        <p>Сценарии жизни</p>
      </div>
      <div class="team-card reveal">
        <div class="team-avatar">SD</div>
        <h4>Пространственный дизайнер</h4>
        <p>Зонирование и навигация</p>
      </div>
      <div class="team-card reveal">
        <div class="team-avatar">PM</div>
        <h4>Проджект-менеджер</h4>
        <p>Управление проектом</p>
      </div>
      <div class="team-card reveal">
        <div class="team-avatar">DA</div>
        <h4>Data-аналитик</h4>
        <p>Метрики и дашборды</p>
      </div>
    </div>
  </div>
</section>

<!-- CTA -->
<section class="cta-section" id="contact">
  <div class="container">
    <span class="section-label reveal" style="color:var(--gold)">Свяжитесь с нами</span>
    <h2 class="section-title reveal">Готовы оживить ваше пространство?</h2>
    <p class="section-intro reveal" style="color:rgba(255,255,255,.75);margin-left:auto;margin-right:auto">Расскажите об объекте — мы предложим первый шаг и покажем, как данные и сценарии могут сделать среду живой.</p>
    <form class="cta-form reveal" onsubmit="event.preventDefault();alert('Спасибо! Мы свяжемся с вами в ближайшее время.');this.reset();">
      <input type="text" placeholder="Ваше имя" required>
      <input type="text" placeholder="Компания" required>
      <input type="tel" placeholder="Телефон" required>
      <input type="email" placeholder="Email" required>
      <textarea placeholder="Коротко об объекте и задаче"></textarea>
      <button type="submit">Обсудить проект</button>
    </form>
  </div>
</section>

<!-- FOOTER -->
<footer>
  <div class="container">
    <div class="footer-grid">
      <div class="footer-brand">
        <a href="#" class="logo">
          <svg viewBox="0 0 520 320"><use href="#logo-mark"/></svg>
          <span>PULSOFT</span>
        </a>
        <p>Пульс твоего пространства. Architecture of behaviour, experience design и урбанистика в одном флаконе.</p>
      </div>
      <div class="footer-col">
        <h4>Навигация</h4>
        <a href="#services">Услуги</a>
        <a href="#audience">Клиенты</a>
        <a href="#why">Почему мы</a>
        <a href="#team">Команда</a>
        <a href="#contact">Контакты</a>
      </div>
      <div class="footer-col">
        <h4>Контакты</h4>
        <a href="tel:+70000000000">+7 (000) 000-00-00</a>
        <a href="mailto:hello@pulsoft.ru">hello@pulsoft.ru</a>
      </div>
    </div>
    <div class="footer-bottom">
      <span>© 2026 Pulsoft. Все права защищены.</span>
      <span>Пульс твоего пространства.</span>
    </div>
  </div>
</footer>

<script>
  // Reveal on scroll
  const io = new IntersectionObserver((entries)=>{
    entries.forEach(e=>{ if(e.isIntersecting){ e.target.classList.add('visible'); io.unobserve(e.target);} });
  },{threshold:.12});
  document.querySelectorAll('.reveal').forEach(el=>io.observe(el));
</script>

</body>
</html>
