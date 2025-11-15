## Hi there 👋

<!--
**fgfghdx88-sudo/fgfghdx88-sudo** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
<!DOCTYPE html>
<html lang="ru" data-theme="dark">
<head>
  <meta charset="UTF-8" />
  <title>Моё творчество</title>
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <style>
    :root {
      --bg: #050509;
      --bg-elevated: #101018;
      --text: #f5f5f7;
      --text-muted: #9b9ca5;
      --accent: #4f46e5;
      --accent-soft: rgba(79, 70, 229, 0.12);
      --border-subtle: rgba(255, 255, 255, 0.06);
      --card-radius: 18px;
      --shadow-soft: 0 18px 45px rgba(0, 0, 0, 0.6);
    }

    [data-theme="light"] {
      --bg: #f5f5f7;
      --bg-elevated: #ffffff;
      --text: #111827;
      --text-muted: #6b7280;
      --accent: #4f46e5;
      --accent-soft: rgba(79, 70, 229, 0.08);
      --border-subtle: rgba(15, 23, 42, 0.08);
      --shadow-soft: 0 18px 45px rgba(15, 23, 42, 0.12);
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: system-ui, -apple-system, BlinkMacSystemFont, "SF Pro Text",
        "Segoe UI", sans-serif;
      background: radial-gradient(circle at top, #111827 0, var(--bg) 40%);
      color: var(--text);
      min-height: 100vh;
      display: flex;
      justify-content: center;
      padding: 24px 12px;
    }

    .shell {
      width: 100%;
      max-width: 1120px;
      background: linear-gradient(
          135deg,
          rgba(255, 255, 255, 0.03),
          rgba(15, 23, 42, 0.5)
        ),
        var(--bg-elevated);
      border-radius: 28px;
      border: 1px solid var(--border-subtle);
      box-shadow: var(--shadow-soft);
      backdrop-filter: blur(26px);
      padding: 20px;
      display: flex;
      flex-direction: column;
      gap: 24px;
    }

    @media (min-width: 900px) {
      .shell {
        padding: 28px 32px;
        margin: 24px 0;
      }
    }

    header {
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 16px;
    }

    .brand {
      display: flex;
      align-items: center;
      gap: 12px;
    }

    .logo {
      width: 36px;
      height: 36px;
      border-radius: 14px;
      background: radial-gradient(circle at 30% 20%, #a855f7, #4f46e5);
      display: flex;
      align-items: center;
      justify-content: center;
      color: white;
      font-weight: 700;
      font-size: 18px;
      box-shadow: 0 12px 30px rgba(79, 70, 229, 0.6);
    }

    .brand-text {
      display: flex;
      flex-direction: column;
      gap: 2px;
    }

    .brand-title {
      font-size: 16px;
      font-weight: 600;
      letter-spacing: 0.03em;
    }

    .brand-sub {
      font-size: 12px;
      color: var(--text-muted);
    }

    nav {
      display: flex;
      align-items: center;
      gap: 8px;
    }

    .nav-link {
      font-size: 13px;
      padding: 7px 12px;
      border-radius: 999px;
      border: 1px solid transparent;
      color: var(--text-muted);
      cursor: pointer;
      background: transparent;
      transition: all 0.25s ease;
    }

    .nav-link:hover {
      color: var(--text);
      border-color: var(--border-subtle);
      background: rgba(148, 163, 184, 0.08);
    }

    .nav-link.active {
      color: var(--text);
      border-color: rgba(79, 70, 229, 0.6);
      background: var(--accent-soft);
    }

    .theme-toggle {
      width: 34px;
      height: 34px;
      border-radius: 999px;
      border: 1px solid var(--border-subtle);
      background: radial-gradient(circle at 30% 0, #ffffff20, #020617);
      display: flex;
      align-items: center;
      justify-content: center;
      cursor: pointer;
      color: var(--text-muted);
      transition: all 0.25s ease;
    }

    .theme-toggle:hover {
      color: var(--text);
      border-color: rgba(79, 70, 229, 0.8);
      background: var(--accent-soft);
      transform: translateY(-1px);
      box-shadow: 0 10px 25px rgba(15, 23, 42, 0.45);
    }

    main {
      display: grid;
      grid-template-columns: minmax(0, 1.5fr) minmax(0, 2fr);
      gap: 24px;
    }

    @media (max-width: 800px) {
      main {
        grid-template-columns: 1fr;
      }
    }

    .hero {
      display: flex;
      flex-direction: column;
      gap: 18px;
    }

    .chip-row {
      display: flex;
      flex-wrap: wrap;
      gap: 8px;
    }

    .chip {
      font-size: 11px;
      padding: 5px 10px;
      border-radius: 999px;
      border: 1px solid rgba(148, 163, 184, 0.25);
      color: var(--text-muted);
      background: rgba(15, 23, 42, 0.6);
    }

    [data-theme="light"] .chip {
      background: rgba(255, 255, 255, 0.9);
    }

    h1 {
      font-size: 26px;
      line-height: 1.2;
      letter-spacing: -0.02em;
    }

    @media (min-width: 900px) {
      h1 {
        font-size: 32px;
      }
    }

    .hero-sub {
      font-size: 14px;
      color: var(--text-muted);
      max-width: 40rem;
    }

    .hero-actions {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
    }

    .btn-primary,
    .btn-ghost {
      font-size: 13px;
      padding: 9px 16px;
      border-radius: 999px;
      border: 1px solid transparent;
      cursor: pointer;
      transition: all 0.22s ease;
      display: inline-flex;
      align-items: center;
      gap: 6px;
      text-decoration: none;
    }

    .btn-primary {
      background: linear-gradient(135deg, #6366f1, #a855f7);
      color: #f9fafb;
      box-shadow: 0 10px 28px rgba(79, 70, 229, 0.7);
    }

    .btn-primary:hover {
      transform: translateY(-1px);
      box-shadow: 0 16px 36px rgba(79, 70, 229, 0.9);
    }

    .btn-ghost {
      border-color: var(--border-subtle);
      color: var(--text-muted);
      background: rgba(15, 23, 42, 0.4);
    }

    [data-theme="light"] .btn-ghost {
      background: rgba(255, 255, 255, 0.9);
    }

    .btn-ghost:hover {
      color: var(--text);
      border-color: rgba(148, 163, 184, 0.6);
      background: rgba(148, 163, 184, 0.12);
    }

    .hero-meta {
      display: flex;
      gap: 18px;
      flex-wrap: wrap;
      margin-top: 8px;
    }

    .meta-item {
      font-size: 11px;
      color: var(--text-muted);
    }

    .meta-label {
      text-transform: uppercase;
      letter-spacing: 0.13em;
      font-weight: 600;
      font-size: 10px;
      opacity: 0.7;
    }

    .meta-value {
      margin-top: 3px;
    }

    .content {
      display: flex;
      flex-direction: column;
      gap: 16px;
    }

    .tabs {
      display: inline-flex;
      padding: 4px;
      border-radius: 999px;
      background: rgba(15, 23, 42, 0.7);
      border: 1px solid rgba(148, 163, 184, 0.3);
      width: fit-content;
    }

    [data-theme="light"] .tabs {
      background: rgba(255, 255, 255, 0.95);
    }

    .tab {
      border-radius: 999px;
      border: none;
      font-size: 12px;
      padding: 6px 12px;
      cursor: pointer;
      color: var(--text-muted);
      background: transparent;
      transition: all 0.22s ease;
      white-space: nowrap;
    }

    .tab.active {
      background: var(--accent-soft);
      color: var(--text);
    }

    .card-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 14px;
    }

    .card {
      position: relative;
      border-radius: var(--card-radius);
      background: linear-gradient(
          135deg,
          rgba(148, 163, 184, 0.08),
          rgba(15, 23, 42, 0.9)
        ),
        var(--bg-elevated);
      border: 1px solid rgba(148, 163, 184, 0.24);
      padding: 14px;
      overflow: hidden;
      cursor: default;
      transition: all 0.26s ease;
    }

    [data-theme="light"] .card {
      background: linear-gradient(
          135deg,
          rgba(148, 163, 184, 0.08),
          rgba(255, 255, 255, 0.98)
        ),
        var(--bg-elevated);
      border-color: rgba(148, 163, 184, 0.3);
    }

    .card:hover {
      transform: translateY(-3px);
      box-shadow: 0 18px 40px rgba(15, 23, 42, 0.7);
      border-color: rgba(79, 70, 229, 0.8);
    }

    .card-tag {
      display: inline-flex;
      font-size: 10px;
      padding: 3px 8px;
      border-radius: 999px;
      background: rgba(15, 23, 42, 0.75);
      color: var(--text-muted);
      border: 1px solid rgba(148, 163, 184, 0.4);
      margin-bottom: 6px;
    }

    [data-theme="light"] .card-tag {
      background: rgba(255, 255, 255, 0.95);
    }

    .card-title {
      font-size: 14px;
      font-weight: 600;
      margin-bottom: 4px;
    }

    .card-desc {
      font-size: 12px;
      color: var(--text-muted);
      margin-bottom: 8px;
    }

    .card-footer {
      font-size: 11px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      color: var(--text-muted);
    }

    .pill {
      padding: 3px 8px;
      border-radius: 999px;
      border: 1px dashed rgba(148, 163, 184, 0.6);
      font-size: 10px;
    }

    .card-accent {
      position: absolute;
      right: -40px;
      top: -40px;
      width: 120px;
      height: 120px;
      border-radius: 50%;
      background: radial-gradient(circle, rgba(79, 70, 229, 0.28), transparent);
      pointer-events: none;
    }

    footer {
      display: flex;
      flex-wrap: wrap;
      justify-content: space-between;
      align-items: center;
      gap: 10px;
      padding-top: 6px;
      border-top: 1px solid var(--border-subtle);
      font-size: 11px;
      color: var(--text-muted);
    }

    .socials {
      display: flex;
      gap: 10px;
      flex-wrap: wrap;
    }

    .social-link {
      color: var(--text-muted);
      text-decoration: none;
      border-bottom: 1px dashed transparent;
      padding-bottom: 1px;
      transition: all 0.18s ease;
    }

    .social-link:hover {
      color: var(--text);
      border-bottom-color: rgba(148, 163, 184, 0.7);
    }

    .hidden {
      display: none !important;
    }
  </style>
</head>
<body>
  <div class="shell">
    <header>
      <div class="brand">
        <div class="logo">M</div>
        <div class="brand-text">
          <div class="brand-title">Моё творчество</div>
          <div class="brand-sub">личное портфолио</div>
        </div>
      </div>
      <nav>
        <button class="nav-link active" data-section="home">Главная</button>
        <button class="nav-link" data-section="portfolio">Портфолио</button>
        <button class="nav-link" data-section="about">Обо мне</button>
        <button class="nav-link" data-section="contacts">Контакты</button>
        <button class="theme-toggle" id="themeToggle" title="Переключить тему">
          ☾
        </button>
      </nav>
    </header>

    <main>
      <section class="hero" id="section-home">
        <div class="chip-row">
          <div class="chip">Открываю мир через творчество</div>
          <div class="chip">Готов к новым проектам</div>
        </div>

        <h1>Портфолио, где каждое произведение говорит само за себя.</h1>

        <p class="hero-sub">
          Здесь собраны лучшие работы: визуал, тексты, идеи и эксперименты. 
          Сайт создан так, чтобы подчёркивать содержание, а не отвлекать от него.
        </p>

        <div class="hero-actions">
          <a href="#" class="btn-primary" data-section-link="portfolio">
            Смотреть работы
          </a>
          <a href="#" class="btn-ghost" data-section-link="contacts">
            Связаться со мной
          </a>
        </div>

        <div class="hero-meta">
          <div class="meta-item">
            <div class="meta-label">Формат</div>
            <div class="meta-value">фото, видео, тексты, эксперименты</div>
          </div>
          <div class="meta-item">
            <div class="meta-label">Обновления</div>
            <div class="meta-value">добавляю новые работы по мере выхода</div>
          </div>
        </div>
      </section>

      <section class="content">
        <div class="tabs">
          <button class="tab active" data-tab="portfolio">Работы</button>
          <button class="tab" data-tab="notes">Заметки</button>
        </div>

        <div id="tab-portfolio">
          <div class="card-grid" id="portfolioGrid">
            <!-- Примеры работ. Меняй/добавляй под себя -->
            <article class="card">
              <div class="card-accent"></div>
              <div class="card-tag">Визуал</div>
              <div class="card-title">Серия «Город будущего»</div>
              <div class="card-desc">
                Подборка работ в стиле sci‑fi: неон, холодные оттенки, минимализм, 
                акцент на атмосфере и характере персонажей.
              </div>
              <div class="card-footer">
                <span class="pill">изображения / концепт-арт</span>
                <span>2024</span>
              </div>
            </article>

            <article class="card">
              <div class="card-accent"></div>
              <div class="card-tag">Видео</div>
              <div class="card-title">Короткие мем‑ролики</div>
              <div class="card-desc">
                10‑секундные ролики с продуманным таймингом шуток, резкой
                динамикой и точным попаданием в звук.
              </div>
              <div class="card-footer">
                <span class="pill">монтаж / звук / идея</span>
                <span>постоянно пополняется</span>
              </div>
            </article>

            <article class="card">
              <div class="card-accent"></div>
              <div class="card-tag">Тексты</div>
              <div class="card-title">Нарративы и концепции</div>
              <div class="card-desc">
                Истории, описания миров и концепции персонажей, 
                которые можно развивать в сценарии, книги или игры.
              </div>
              <div class="card-footer">
                <span class="pill">сторителлинг</span>
                <span>выборочно</span>
              </div>
            </article>
          </div>
        </div>

        <div id="tab-notes" class="hidden">
          <div class="card">
            <div class="card-accent"></div>
            <div class="card-tag">Заметки</div>
            <div class="card-title">Как устроен этот сайт</div>
            <div class="card-desc">
              Сайт сделан так, чтобы его легко было дополнять. 
              Достаточно открыть файл <b>index.html</b>, найти блок
              <code>&lt;div id="portfolioGrid"&gt;...&lt;/div&gt;</code> 
              и добавить туда ещё один блок <code>&lt;article class="card"&gt;...&lt;/article&gt;</code>.
            </div>
            <div class="card-footer">
              <span class="pill">управление через код</span>
              <span>редактируй как конструктор</span>
            </div>
          </div>
        </div>

        <!-- Секции для навигации -->
        <section id="section-portfolio" class="">
          <!-- Здесь уже есть карточки выше, 
               эта секция просто якорь для скролла -->
        </section>

        <section id="section-about" class="hidden">
          <div class="card">
            <div class="card-accent"></div>
            <div class="card-tag">Обо мне</div>
            <div class="card-title">Кто стоит за этим портфолио</div>
            <div class="card-desc">
              Здесь можно написать пару абзацев о себе: чем занимаешься, 
              что тебе интересно, какие направления творчества тебе ближе всего. 
              Можно упомянуть инструменты, с которыми работаешь, 
              и то, что сейчас в фокусе.
            </div>
            <div class="card-footer">
              <span class="pill">творчество / эксперименты</span>
              <span>обнови текст под себя</span>
            </div>
          </div>
        </section>

        <section id="section-contacts" class="hidden">
          <div class="card">
            <div class="card-accent"></div>
            <div class="card-tag">Контакты</div>
            <div class="card-title">Как со мной связаться</div>
            <div class="card-desc">
              Оставь здесь удобные каналы связи: Telegram, VK, почта или другие платформы.
            </div>
            <div class="card-footer">
              <span class="pill">открыт к предложениям</span>
              <span>ответ — по возможности</span>
            </div>
          </div>
        </section>
      </section>
    </main>

    <footer>
      <span>© <span id="year"></span> Моё творчество. Все права защищены.</span>
      <div class="socials">
        <a href="https://t.me/" target="_blank" class="social-link">Telegram</a>
        <a href="#" class="social-link">VK</a>
        <a href="mailto:example@email.com" class="social-link">Email</a>
      </div>
    </footer>
  </div>

  <script>
    const root = document.documentElement;
    const themeToggle = document.getElementById("themeToggle");

    function setTheme(theme) {
      root.setAttribute("data-theme", theme);
      localStorage.setItem("theme", theme);
      themeToggle.textContent = theme === "dark" ? "☾" : "☼";
    }

    const savedTheme = localStorage.getItem("theme");
    if (savedTheme === "light" || savedTheme === "dark") {
      setTheme(savedTheme);
    } else {
      const prefersDark = window.matchMedia &&
        window.matchMedia("(prefers-color-scheme: dark)").matches;
      setTheme(prefersDark ? "dark" : "light");
    }

    themeToggle.addEventListener("click", () => {
      const current = root.getAttribute("data-theme");
      setTheme(current === "dark" ? "light" : "dark");
    });

    const navLinks = document.querySelectorAll(".nav-link");
    const sections = {
      home: document.getElementById("section-home"),
      portfolio: document.getElementById("section-portfolio"),
      about: document.getElementById("section-about"),
      contacts: document.getElementById("section-contacts"),
    };

    function showSection(key) {
      Object.keys(sections).forEach((k) => {
        if (!sections[k]) return;
        if (k === key || (key === "home" && k === "home")) {
          sections[k].classList.remove("hidden");
          if (k === "home") {
            window.scrollTo({ top: 0, behavior: "smooth" });
          } else {
            sections[k].scrollIntoView({ behavior: "smooth", block: "start" });
          }
        } else if (k !== "home") {
          sections[k].classList.add("hidden");
        }
      });

      navLinks.forEach((btn) =>
        btn.classList.toggle("active", btn.dataset.section === key)
      );
    }

    navLinks.forEach((btn) => {
      btn.addEventListener("click", () => {
        showSection(btn.dataset.section);
      });
    });

    document.querySelectorAll("[data-section-link]").forEach((link) => {
      link.addEventListener("click", (e) => {
        e.preventDefault();
        const key = link.dataset.sectionLink;
        showSection(key);
      });
    });

    const tabs = document.querySelectorAll(".tab");
    const tabPortfolio = document.getElementById("tab-portfolio");
    const tabNotes = document.getElementById("tab-notes");

    tabs.forEach((tab) => {
      tab.addEventListener("click", () => {
        tabs.forEach((t) => t.classList.remove("active"));
        tab.classList.add("active");

        const key = tab.dataset.tab;
        if (key === "portfolio") {
          tabPortfolio.classList.remove("hidden");
          tabNotes.classList.add("hidden");
        } else {
          tabNotes.classList.remove("hidden");
          tabPortfolio.classList.add("hidden");
        }
      });
    });

    document.getElementById("year").textContent = new Date().getFullYear();
  </script>
</body>
</html>
