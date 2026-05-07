<!doctype html>
<html lang="ru">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>TASVER — кадровое агентство (Москва)</title>
  <meta name="description" content="TASVER — подбор персонала для работодателей и трудоустройство для соискателей в Москве." />
  <style>
    :root {
      --bg: #f8f9fb;
      --card: #ffffff;
      --text: #1a1d2e;
      --muted: #6b7280;
      --accent: #4f46e5;
      --accent2: #10b981;
      --border: rgba(0, 0, 0, 0.06);
      --shadow: 0 1px 3px rgba(0, 0, 0, 0.04), 0 1px 2px rgba(0, 0, 0, 0.06);
      --shadow-lg: 0 10px 40px rgba(0, 0, 0, 0.08);
      --radius: 12px;
    }
    * {
      box-sizing: border-box;
    }
    body {
      margin: 0;
      font-family: 'Inter', ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, 'Helvetica Neue', Arial, sans-serif;
      background: var(--bg);
      color: var(--text);
      line-height: 1.6;
      -webkit-font-smoothing: antialiased;
    }
    a {
      color: inherit;
      text-decoration: none;
    }
    .container {
      max-width: 1200px;
      margin: 0 auto;
      padding: 0 24px;
    }
  
    /* Header */
    header {
      position: sticky;
      top: 0;
      z-index: 50;
      backdrop-filter: blur(20px);
      background: rgba(248, 249, 251, 0.85);
      border-bottom: 1px solid var(--border);
    }
    .nav {
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 16px 0;
      gap: 24px;
    }
    .brand {
      display: flex;
      align-items: center;
      gap: 12px;
      min-width: 200px;
    }
    .logo {
      width: 42px;
      height: 42px;
      border-radius: 10px;
      background: linear-gradient(135deg, #4f46e5, #7c3aed);
      display: grid;
      place-items: center;
      font-weight: 800;
      font-size: 20px;
      color: white;
      letter-spacing: 0.5px;
      box-shadow: 0 4px 12px rgba(79, 70, 229, 0.3);
    }
    .brand .name {
      font-weight: 700;
      font-size: 20px;
      letter-spacing: -0.3px;
    }
    .brand .sub {
      color: var(--muted);
      font-size: 12px;
      margin-top: 2px;
    }
    .menu {
      display: flex;
      gap: 4px;
      flex-wrap: wrap;
      justify-content: flex-end;
    }
    .menu a {
      color: var(--muted);
      padding: 8px 14px;
      border-radius: 8px;
      transition: 0.15s;
      font-weight: 500;
      font-size: 14px;
    }
    .menu a:hover {
      background: rgba(0, 0, 0, 0.04);
      color: var(--text);
    }
    .cta {
      display: flex;
      align-items: center;
      gap: 8px;
    }
    
    /* Buttons */
    .btn {
      border: 1px solid var(--border);
      background: var(--card);
      color: var(--text);
      padding: 10px 18px;
      border-radius: 8px;
      font-weight: 600;
      font-size: 14px;
      cursor: pointer;
      transition: 0.15s;
      display: inline-flex;
      align-items: center;
      gap: 8px;
      white-space: nowrap;
      box-shadow: var(--shadow);
    }
    .btn:hover {
      transform: translateY(-1px);
      box-shadow: var(--shadow-lg);
    }
    .btn-accent {
      background: var(--accent);
      border-color: var(--accent);
      color: white;
      box-shadow: 0 4px 14px rgba(79, 70, 229, 0.25);
    }
    .btn-accent:hover {
      background: #4338ca;
      border-color: #4338ca;
    }
    
    /* Sections */
    main section {
      padding: 80px 0;
    }
    .hero {
      padding: 60px 0 40px;
    }
    .hero-grid {
      display: grid;
      grid-template-columns: 1.1fr 0.9fr;
      gap: 32px;
      align-items: start;
    }
    @media (max-width: 900px) {
      .hero-grid {
        grid-template-columns: 1fr;
      }
      .brand {
        min-width: auto;
      }
      .menu {
        display: none;
      }
    }
    
    /* Cards */
    .hero-card {
      background: var(--card);
      border: 1px solid var(--border);
      border-radius: var(--radius);
      padding: 40px;
      box-shadow: var(--shadow-lg);
    }
    .kicker {
      display: inline-flex;
      align-items: center;
      gap: 8px;
      padding: 6px 14px;
      border-radius: 20px;
      background: #eef2ff;
      color: #4f46e5;
      font-weight: 600;
      font-size: 13px;
    }
    .dot {
      width: 8px;
      height: 8px;
      border-radius: 50%;
      background: #10b981;
      box-shadow: 0 0 0 4px rgba(16, 185, 129, 0.15);
    }
    h1 {
      margin: 20px 0 16px;
      font-size: 48px;
      line-height: 1.1;
      letter-spacing: -1px;
      font-weight: 800;
    }
    @media (max-width: 520px) {
      h1 {
        font-size: 34px;
      }
    }
    .lead {
      color: var(--muted);
      font-size: 17px;
      margin: 0 0 24px;
      max-width: 60ch;
      line-height: 1.7;
    }
    .hero-actions {
      display: flex;
      gap: 12px;
      flex-wrap: wrap;
      margin-top: 24px;
    }
    .stats {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 12px;
      margin-top: 28px;
    }
    .stat {
      background: #f8f9fb;
      border: 1px solid var(--border);
      border-radius: 10px;
      padding: 16px;
    }
    .stat .num {
      font-weight: 800;
      font-size: 22px;
      color: var(--accent);
    }
    .stat .lbl {
      color: var(--muted);
      font-size: 13px;
      margin-top: 4px;
    }
    .side {
      display: flex;
      flex-direction: column;
      gap: 16px;
    }
    .panel {
      background: var(--card);
      border: 1px solid var(--border);
      border-radius: var(--radius);
      padding: 24px;
      box-shadow: var(--shadow);
    }
    .panel h3 {
      margin: 0 0 12px;
      font-size: 18px;
      font-weight: 700;
    }
    .list {
      margin: 0;
      padding-left: 20px;
      color: var(--muted);
      line-height: 2;
    }
    .list li {
      margin: 4px 0;
    }
    
    /* Grids */
    .grid-3 {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 20px;
    }
    @media (max-width: 900px) {
      .grid-3 {
        grid-template-columns: 1fr;
      }
    }
    .card {
      background: var(--card);
      border: 1px solid var(--border);
      border-radius: var(--radius);
      padding: 28px;
      box-shadow: var(--shadow);
      transition: 0.2s;
    }
    .card:hover {
      box-shadow: var(--shadow-lg);
      transform: translateY(-2px);
    }
    .card .title {
      font-weight: 700;
      font-size: 18px;
      margin-bottom: 10px;
    }
    .card .desc {
      color: var(--muted);
      margin: 0;
      line-height: 1.7;
    }
    .section-title {
      display: flex;
      align-items: flex-end;
      justify-content: space-between;
      gap: 16px;
      margin-bottom: 32px;
    }
    .section-title h2 {
      margin: 0 0 8px;
      font-size: 32px;
      font-weight: 800;
      letter-spacing: -0.5px;
    }
    .section-title p {
      margin: 0;
      color: var(--muted);
      max-width: 60ch;
      font-size: 16px;
    }
    
    /* Steps */
    .steps {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 20px;
    }
    @media (max-width: 900px) {
      .steps {
        grid-template-columns: 1fr;
      }
    }
    .step {
      background: var(--card);
      border: 1px solid var(--border);
      border-radius: var(--radius);
      padding: 28px;
      position: relative;
      box-shadow: var(--shadow);
      transition: 0.2s;
    }
    .step:hover {
      box-shadow: var(--shadow-lg);
      transform: translateY(-2px);
    }
    .step .n {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      width: 40px;
      height: 40px;
      border-radius: 10px;
      background: #eef2ff;
      color: #4f46e5;
      font-weight: 800;
      font-size: 18px;
      margin-bottom: 16px;
    }
    .step h4 {
      margin: 0 0 10px;
      font-size: 17px;
      font-weight: 700;
    }
    .step p {
      margin: 0;
      color: var(--muted);
      line-height: 1.7;
    }
    
    /* Contact */
    .contact-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 24px;
      align-items: start;
    }
    @media (max-width: 900px) {
      .contact-grid {
        grid-template-columns: 1fr;
      }
    }
    form {
      display: grid;
      gap: 12px;
      margin-top: 12px;
    }
    input, textarea {
      width: 100%;
      padding: 12px 16px;
      border-radius: 8px;
      border: 1px solid var(--border);
      background: #f8f9fb;
      color: var(--text);
      outline: none;
      font-size: 15px;
      font-family: inherit;
      transition: 0.15s;
    }
    input:focus, textarea:focus {
      border-color: #4f46e5;
      box-shadow: 0 0 0 3px rgba(79, 70, 229, 0.1);
      background: white;
    }
    textarea {
      min-height: 120px;
      resize: vertical;
    }
    input::placeholder, textarea::placeholder {
      color: #9ca3af;
    }
    .fineprint {
      color: var(--muted);
      font-size: 12px;
      margin-top: 4px;
      line-height: 1.5;
    }
    
    /* Footer */
    .footer {
      padding: 32px 0;
      border-top: 1px solid var(--border);
      color: var(--muted);
      font-size: 14px;
    }
    .footer .row {
      display: flex;
      justify-content: space-between;
      gap: 12px;
      flex-wrap: wrap;
      align-items: center;
    }
    
    /* Table */
    table {
      width: 100%;
      border-collapse: collapse;
      background: white;
      border: 1px solid var(--border);
      border-radius: var(--radius);
      overflow: hidden;
    }
    th, td {
      padding: 12px 16px;
      border-bottom: 1px solid var(--border);
      vertical-align: top;
    }
    th {
      width: 35%;
      color: var(--muted);
      font-weight: 600;
      background: #f8f9fb;
    }
    tr:last-child td, tr:last-child th {
      border-bottom: none;
    }
    .small-muted {
      font-size: 12px;
      color: var(--muted);
      margin-top: 12px;
    }
  </style>
</head>
<body>

<header>
  <div class="container">
    <div class="nav">
      <a class="brand" href="#top" aria-label="TASVER">
        <div class="logo">T</div>
        <div>
          <div class="name">TASVER</div>
          <div class="sub">Кадровое агентство • Москва</div>
        </div>
      </a>

      <nav class="menu" aria-label="Навигация">
        <a href="#services">Услуги</a>
        <a href="#employers">Работодателям</a>
        <a href="#candidates">Соискателям</a>
        <a href="#process">Как работаем</a>
        <a href="#requisites">Реквизиты</a>
        <a href="#contacts">Контакты</a>
      </nav>

      <div class="cta">
        <a class="btn" href="tel:+79166661266">📞 +7 (916) 666-12-66</a>
        <a class="btn btn-accent" href="#contacts">Оставить заявку</a>
      </div>
    </div>
  </div>
</header>

<main id="top">
  <!-- HERO -->
  <section class="hero">
    <div class="container">
      <div class="hero-grid">
        <div class="hero-card">
          <div class="kicker"><span class="dot"></span> Подбор персонала под ваши задачи</div>
          <h1>Найдём сотрудников и закроем вакансии в Москве</h1>
          <p class="lead">
            TASVER помогает работодателям быстро и качественно подбирать персонал,
            а соискателям — находить подходящие вакансии и получать поддержку на каждом этапе.
          </p>
          <div class="hero-actions">
            <a class="btn btn-accent" href="#contacts">Запросить подбор</a>
            <a class="btn" href="#candidates">Хочу работу</a>
          </div>
          <div class="stats">
            <div class="stat">
              <div class="num">Быстро</div>
              <div class="lbl">короткие сроки подбора</div>
            </div>
            <div class="stat">
              <div class="num">Точно</div>
              <div class="lbl">под требования работодателя</div>
            </div>
          </div>
        </div>

        <div class="side">
          <div class="panel">
            <h3>Что предлагаем</h3>
            <ul class="list">
              <li>Подбор персонала (офис, продажи, производство)</li>
              <li>Массовый подбор (если нужно закрыть много вакансий)</li>
              <li>Сопровождение и консультации по найму</li>
            </ul>
          </div>
          <div class="panel">
            <h3>Контакты</h3>
            <ul class="list">
              <li><b>Москва</b></li>
              <li><a href="tel:+79166661266"><b>+7 (916) 666-12-66</b></a></li>
              <li><a href="mailto:tasver@tasver.ru"><b>tasver@tasver.ru</b></a></li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- SERVICES -->
  <section id="services">
    <div class="container">
      <div class="section-title">
        <div>
          <h2>Услуги TASVER</h2>
          <p>Подбираем персонал системно: от согласования требований до финального кандидата.</p>
        </div>
      </div>

      <div class="grid-3">
        <div class="card">
          <div class="title">Подбор персонала</div>
          <p class="desc">Подберём кандидатов под ваши компетенции, график, опыт и уровень дохода.</p>
        </div>
        <div class="card">
          <div class="title">Массовый подбор</div>
          <p class="desc">Помогаем закрывать объёмы вакансий: быстрый поток кандидатов и контроль качества.</p>
        </div>
        <div class="card">
          <div class="title">Кадровый консалтинг</div>
          <p class="desc">Рекомендации по структуре отбора, профилю должности и улучшению процесса найма.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- EMPLOYERS -->
  <section id="employers">
    <div class="container">
      <div class="section-title">
        <div>
          <h2>Работодателям</h2>
          <p>Если нужно закрыть вакансию быстро и без "мимо" — мы возьмём процесс на себя.</p>
        </div>
      </div>

      <div class="grid-3">
        <div class="card">
          <div class="title">Согласуем требования</div>
          <p class="desc">Соберём профиль кандидата: обязанности, навыки, опыт, сроки, бюджет.</p>
        </div>
        <div class="card">
          <div class="title">Отбор и проверка</div>
          <p class="desc">Фильтрация резюме, интервью, уточнение мотивации и соответствия требованиям.</p>
        </div>
        <div class="card">
          <div class="title">Представим кандидатов</div>
          <p class="desc">Передадим короткий список и поможем с финальным выбором.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- CANDIDATES -->
  <section id="candidates">
    <div class="container">
      <div class="section-title">
        <div>
          <h2>Соискателям</h2>
          <p>Откликайтесь — подберём вакансии под ваш опыт и цели.</p>
        </div>
      </div>

      <div class="grid-3">
        <div class="card">
          <div class="title">Подбор вакансий</div>
          <p class="desc">Предложим варианты, которые соответствуют вашим навыкам и ожиданиям.</p>
        </div>
        <div class="card">
          <div class="title">Подготовка к собеседованию</div>
          <p class="desc">Подскажем, как лучше презентовать опыт и на что обратить внимание.</p>
        </div>
        <div class="card">
          <div class="title">Сопровождение</div>
          <p class="desc">Держим связь на этапах, чтобы вы не "терялись" в процессе.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- PROCESS -->
  <section id="process">
    <div class="container">
      <div class="section-title">
        <div>
          <h2>Как мы работаем</h2>
          <p>Прозрачный процесс подбора: быстро, аккуратно, с контролем качества на каждом шаге.</p>
        </div>
      </div>

      <div class="steps">
        <div class="step">
          <div class="n">1</div>
          <h4>Заявка</h4>
          <p>Оставляете запрос по вакансии или информацию о себе.</p>
        </div>
        <div class="step">
          <div class="n">2</div>
          <h4>Требования</h4>
          <p>Согласуем критерии и сроки (работодатели) / профиль (соискатели).</p>
        </div>
        <div class="step">
          <div class="n">3</div>
          <h4>Подбор кандидатов</h4>
          <p>Поиск, отбор, интервью и проверка соответствия.</p>
        </div>
        <div class="step">
          <div class="n">4</div>
          <h4>Результат</h4>
          <p>Передаём кандидатов / предлагаем вакансии, сопровождаем до решения.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- CONTACTS -->
  <section id="contacts">
    <div class="container">
      <div class="section-title">
        <div>
          <h2>Контакты и заявка</h2>
          <p>Заполните форму — мы свяжемся с вами. (Заявка уходит в Telegram-бот.)</p>
        </div>
      </div>

      <div class="contact-grid">
        <div class="panel">
          <h3>Связаться</h3>
          <ul class="list">
            <li><b>Город:</b> Москва</li>
            <li><b>Телефон:</b> <a href="tel:+79166661266">+7 (916) 666-12-66</a></li>
            <li><b>Email:</b> <a href="mailto:tasver@tasver.ru">tasver@tasver.ru</a></li>
          </ul>

          <div style="margin-top: 24px; padding-top: 24px; border-top: 1px solid var(--border);">
            <h3 style="margin: 0 0 12px; font-size: 16px;">Реквизиты</h3>
            <ul class="list">
              <li><b>ИП:</b> Лебединский Павел Павлович</li>
              <li><b>Адрес:</b> г. Москва, Варшавское шоссе, влд. 132/2</li>
              <li><b>ИНН:</b> 770171269799</li>
              <li><b>ОГРНИП:</b> 316774600133130</li>
              <li><b>р/с:</b> 40802810600000130574</li>
              <li><b>Банк:</b> ПАО «Промсвязьбанк», г. Москва</li>
              <li><b>БИК:</b> 044525555</li>
              <li><b>к/с:</b> 30101810400000000555</li>
            </ul>
          </div>

          <p class="fineprint">Можете написать нам в удобное время. Ответим максимально быстро.</p>
        </div>

        <div class="panel">
          <h3>Оставить заявку</h3>

          <form id="leadForm">
            <input type="text" name="name" placeholder="Ваше имя" required>
            <input type="tel" name="phone" placeholder="Телефон / WhatsApp" required>
            <input type="email" name="email" placeholder="Email (необязательно)">
            <textarea name="message" placeholder="Сообщение: вакансия или ваши данные (опыт, должность, график)..." required></textarea>

            <button class="btn btn-accent" type="submit" style="width: 100%; justify-content: center; padding: 14px;">
              Отправить заявку
            </button>
            <div class="fineprint">Нажимая "Отправить", вы даёте согласие на обработку данных.</div>
          </form>
        </div>
      </div>
    </div>
  </section>
</main>

<footer class="footer">
  <div class="container">
    <div class="row">
      <div>© <span id="y"></span> TASVER. Все права защищены.</div>
      <div>Москва • Подбор персонала • <a href="mailto:tasver@tasver.ru">tasver@tasver.ru</a></div>
    </div>
  </div>
</footer>

<script>
  document.getElementById('y').textContent = new Date().getFullYear();

  const SCRIPT_URL =
    "https://script.google.com/macros/s/AKfycbzIkFId0ivjrZjrlU9rI7OEYXjN2AuDTiIhW5oqMgt-MOdHWrsoPIJe-tAtgKGW9It9IQ/exec";

  const form = document.getElementById("leadForm");
  form.addEventListener("submit", async (e) => {
    e.preventDefault();

    const elements = form.elements;
    const data = {
      name: elements.namedItem("name").value.trim(),
      phone: elements.namedItem("phone").value.trim(),
      email: elements.namedItem("email").value.trim(),
      message: elements.namedItem("message").value.trim()
    };

    try {
      const resp = await fetch(SCRIPT_URL, {
        method: "POST",
        headers: {"Content-Type":"application/json"},
        body: JSON.stringify(data)
      });

      if (!resp.ok) throw new Error("Bad response");

      alert("Спасибо! Заявка отправлена в Telegram. Мы свяжемся с вами.");
      form.reset();
    } catch (err) {
      alert("Не удалось отправить заявку. Попробуйте ещё раз.");
      console.error(err);
    }
  });
</script>

</body>
</html>
