<!doctype html>
<html lang="ru">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>TASVER — кадровое агентство (Москва)</title>
  <meta name="description" content="TASVER — подбор персонала для работодателей и трудоустройство для соискателей в Москве." />
  <style>
    :root{
      --bg:#0b1220;
      --card:#111a2e;
      --text:#e8eefc;
      --muted:#a8b3d6;
      --accent:#ff7a18;
      --accent2:#2dd4bf;
      --border:rgba(255,255,255,.08);
      --shadow:0 16px 50px rgba(0,0,0,.35);
      --radius:18px;
    }
    *{box-sizing:border-box}
    body{
      margin:0;
      font-family: ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, Arial, "Noto Sans", "Liberation Sans", sans-serif;
      background: radial-gradient(1000px 500px at 10% -10%, rgba(255,122,24,.25), transparent 60%),
                  radial-gradient(800px 450px at 100% 0%, rgba(45,212,191,.18), transparent 55%),
                  var(--bg);
      color:var(--text);
      line-height:1.4;
    }
    a{color:inherit; text-decoration:none}
    .container{max-width:1100px; margin:0 auto; padding:0 18px}
    header{
      position:sticky; top:0; z-index:50;
      backdrop-filter: blur(10px);
      background: rgba(11,18,32,.75);
      border-bottom:1px solid var(--border);
    }
    .nav{
      display:flex; align-items:center; justify-content:space-between;
      padding:14px 0;
      gap:14px;
    }
    .brand{
      display:flex; align-items:center; gap:12px;
      min-width: 220px;
    }
    .logo{
      width:40px; height:40px; border-radius:12px;
      background: linear-gradient(135deg, rgba(255,122,24,.95), rgba(45,212,191,.9));
      box-shadow: 0 12px 30px rgba(255,122,24,.22);
      display:grid; place-items:center;
      font-weight:900; letter-spacing:.5px;
    }
    .brand .name{font-weight:850; letter-spacing:.2px}
    .brand .sub{color:var(--muted); font-size:12px; margin-top:2px}
    .menu{
      display:flex; gap:16px; flex-wrap:wrap; justify-content:flex-end;
    }
    .menu a{
      color:var(--muted);
      padding:10px 10px;
      border-radius:10px;
      transition:.2s;
      font-weight:600;
      font-size:14px;
    }
    .menu a:hover{background:rgba(255,255,255,.06); color:var(--text)}
    .cta{
      display:flex; align-items:center; gap:10px;
    }
    .btn{
      border:1px solid rgba(255,255,255,.14);
      background: rgba(255,255,255,.04);
      color:var(--text);
      padding:10px 14px;
      border-radius:12px;
      font-weight:800;
      cursor:pointer;
      transition:.2s;
      display:inline-flex; align-items:center; gap:10px;
      white-space:nowrap;
    }
    .btn:hover{transform: translateY(-1px); border-color:rgba(255,255,255,.22); background: rgba(255,255,255,.06)}
    .btn-accent{
      background: linear-gradient(135deg, rgba(255,122,24,.95), rgba(255,122,24,.75));
      border-color: rgba(255,122,24,.6);
      box-shadow: 0 14px 40px rgba(255,122,24,.2);
    }
    .btn-accent:hover{background: linear-gradient(135deg, rgba(255,122,24,1), rgba(255,122,24,.8))}
    main section{padding:56px 0}
    .hero{
      padding:42px 0 14px;
    }
    .hero-grid{
      display:grid;
      grid-template-columns: 1.1fr .9fr;
      gap:22px;
      align-items:stretch;
    }
    @media (max-width: 900px){
      .hero-grid{grid-template-columns:1fr}
      .brand{min-width:auto}
      .menu{display:none}
    }
    .hero-card{
      background: linear-gradient(180deg, rgba(255,255,255,.05), rgba(255,255,255,.02));
      border:1px solid var(--border);
      border-radius: var(--radius);
      padding:26px;
      box-shadow: var(--shadow);
    }
    .kicker{
      display:inline-flex; align-items:center; gap:10px;
      padding:8px 12px;
      border-radius:999px;
      border:1px solid rgba(255,255,255,.12);
      background: rgba(255,255,255,.03);
      color:var(--muted);
      font-weight:700;
      font-size:13px;
    }
    .dot{
      width:10px; height:10px; border-radius:50%;
      background: var(--accent2);
      box-shadow:0 0 0 6px rgba(45,212,191,.12);
    }
    h1{
      margin:14px 0 10px;
      font-size:44px;
      line-height:1.05;
      letter-spacing:-.6px;
    }
    @media (max-width: 520px){ h1{font-size:34px} }
    .lead{color:var(--muted); font-size:16px; margin:0 0 18px; max-width: 62ch}
    .hero-actions{display:flex; gap:12px; flex-wrap:wrap; margin-top:16px}
    .stats{
      display:grid;
      grid-template-columns: repeat(2, 1fr);
      gap:12px;
      margin-top:18px;
    }
    .stat{
      background: rgba(255,255,255,.03);
      border:1px solid var(--border);
      border-radius: 16px;
      padding:14px;
    }
    .stat .num{font-weight:950; font-size:20px}
    .stat .lbl{color:var(--muted); font-size:13px; margin-top:4px}
    .side{
      display:flex;
      flex-direction:column;
      gap:14px;
    }
    .panel{
      background: rgba(255,255,255,.03);
      border:1px solid var(--border);
      border-radius: var(--radius);
      padding:18px;
      box-shadow: var(--shadow);
    }
    .panel h3{margin:0 0 8px; font-size:18px}
    .list{margin:0; padding-left:18px; color:var(--muted)}
    .list li{margin:8px 0}
    .grid-3{
      display:grid;
      grid-template-columns: repeat(3, 1fr);
      gap:14px;
    }
    @media (max-width: 900px){ .grid-3{grid-template-columns:1fr} }
    .card{
      background: rgba(255,255,255,.03);
      border:1px solid var(--border);
      border-radius: var(--radius);
      padding:18px;
      min-height: 140px;
    }
    .card .title{font-weight:900; margin-bottom:8px}
    .card .desc{color:var(--muted); margin:0}
    .section-title{
      display:flex; align-items:flex-end; justify-content:space-between; gap:12px;
      margin-bottom:18px;
    }
    .section-title h2{
      margin:0;
      font-size:28px;
      letter-spacing:-.3px;
    }
    .section-title p{margin:0; color:var(--muted); max-width: 62ch}
    .steps{
      display:grid; grid-template-columns: repeat(4, 1fr); gap:14px;
    }
    @media (max-width: 900px){ .steps{grid-template-columns:1fr} }
    .step{
      background: rgba(255,255,255,.03);
      border:1px solid var(--border);
      border-radius: var(--radius);
      padding:18px;
      position:relative;
      overflow:hidden;
    }
    .step:after{
      content:"";
      position:absolute; inset:auto -40px -60px auto;
      width:120px; height:120px;
      background: radial-gradient(circle at 30% 30%, rgba(255,122,24,.35), transparent 55%);
      transform: rotate(20deg);
    }
    .step .n{
      display:inline-flex; align-items:center; justify-content:center;
      width:36px; height:36px; border-radius:12px;
      background: rgba(255,122,24,.16);
      border:1px solid rgba(255,122,24,.35);
      font-weight:950;
      margin-bottom:10px;
    }
    .step h4{margin:0 0 8px; font-size:16px}
    .step p{margin:0; color:var(--muted)}
    .contact-grid{
      display:grid; grid-template-columns: 1fr 1fr; gap:14px;
      align-items:start;
    }
    @media (max-width: 900px){ .contact-grid{grid-template-columns:1fr} }
    form{
      display:grid; gap:10px;
      margin-top:10px;
    }
    input, textarea{
      width:100%;
      padding:12px 12px;
      border-radius: 14px;
      border:1px solid rgba(255,255,255,.14);
      background: rgba(0,0,0,.18);
      color: var(--text);
      outline:none;
      font-size:15px;
    }
    textarea{min-height:110px; resize: vertical}
    input::placeholder, textarea::placeholder{color: rgba(168,179,214,.7)}
    .fineprint{color:var(--muted); font-size:12px; margin-top:6px}
    .footer{
      padding:26px 0 40px;
      border-top:1px solid var(--border);
      color:var(--muted);
      font-size:13px;
    }
    .footer .row{
      display:flex; justify-content:space-between; gap:12px; flex-wrap:wrap;
      align-items:center;
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
          <p>Если нужно закрыть вакансию быстро и без “мимо” — мы возьмём процесс на себя.</p>
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
          <p class="desc">Держим связь на этапах, чтобы вы не “терялись” в процессе.</p>
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
          <p>Заполните форму — мы свяжемся с вами. (Телефон и почта указаны ниже.)</p>
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
          <p class="fineprint">Можете написать нам в удобное время. Ответим максимально быстро.</p>
        </div>

        <div class="panel">
          <h3>Оставить заявку</h3>
          <!-- ВНИМАНИЕ: форма пока просто “демо”. Ниже дам как сделать отправку на email/Telegram -->
           <form id="leadForm">
  <input type="text" name="name" placeholder="Ваше имя" required>
  <input type="tel" name="phone" placeholder="Телефон / WhatsApp" required>
  <input type="email" name="email" placeholder="Email (необязательно)">
  <textarea name="message" placeholder="Сообщение: вакансия или ваши данные (опыт, должность, график)..." required></textarea>

  <button class="btn btn-accent" type="submit">Отправить</button>
  <div class="fineprint">Нажимая “Отправить”, вы даёте согласие на обработку данных.</div>
</form>

<script>
  const SCRIPT_URL = "https://script.google.com/macros/s/AKfycbzIkFId0ivjrZjrlU9rI7OEYXjN2AuDTiIhW5oqMgt-MOdHWrsoPIJe-tAtgKGW9It9IQ/exec";

  document.getElementById("leadForm").addEventListener("submit", async (e) => {
    e.preventDefault();

    const form = e.target;
    const data = {
      name: form.name.value.trim(),
      phone: form.phone.value.trim(),
      email: form.email.value.trim(),
      message: form.message.value.trim()
    };

    try {
      const resp = await fetch(SCRIPT_URL, {
        method: "POST",
        headers: { "Content-Type": "application/json" },
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
            <input type="text" name="name" placeholder="Ваше имя" required>
            <input type="tel" name="phone" placeholder="Телефон / WhatsApp" required>
            <input type="email" name="email" placeholder="Email (необязательно)">
            <textarea name="message" placeholder="Сообщение: вакансия или ваши данные (опыт, должность, график)..." required></textarea>
            <button class="btn btn-accent" type="submit">Отправить</button>
            <div class="fineprint">Нажимая “Отправить”, вы даёте согласие на обработку данных.</div>
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
</script>

</body>
</html>
