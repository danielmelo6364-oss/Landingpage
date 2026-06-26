<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Géor | Prata 925 & Acessórios</title>
  <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,600;1,300;1,400&family=Montserrat:wght@300;400;500&display=swap" rel="stylesheet"/>
  <style>
    *, *::before, *::after {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    :root {
      --rose: #c9917a;
      --rose-light: #e8c4b4;
      --rose-dark: #a36b56;
      --rose-bg: #fdf5f2;
      --rose-mid: #f3ddd5;
      --gold: #c8a882;
      --text-dark: #2e2020;
      --text-mid: #6b4c45;
      --text-light: #a08880;
      --white: #ffffff;
    }

    html, body {
      height: 100%;
    }

    body {
      font-family: 'Montserrat', sans-serif;
      background-color: var(--rose-bg);
      color: var(--text-dark);
      min-height: 100vh;
      display: flex;
      flex-direction: column;
    }

    /* ── HEADER ── */
    header {
      text-align: center;
      padding: 48px 24px 32px;
      background: linear-gradient(160deg, var(--rose-mid) 0%, var(--rose-bg) 100%);
      border-bottom: 1px solid var(--rose-light);
    }

    .brand-line {
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 16px;
      margin-bottom: 8px;
    }

    .brand-line::before,
    .brand-line::after {
      content: '';
      display: block;
      width: 48px;
      height: 1px;
      background: var(--rose);
      opacity: 0.6;
    }

    .brand {
      font-family: 'Cormorant Garamond', serif;
      font-size: 48px;
      font-weight: 300;
      letter-spacing: 10px;
      color: var(--rose-dark);
      text-transform: uppercase;
    }

    .brand-sub {
      font-family: 'Cormorant Garamond', serif;
      font-size: 13px;
      letter-spacing: 4px;
      color: var(--text-light);
      text-transform: uppercase;
      font-weight: 400;
      margin-top: 4px;
    }

    /* ── HERO ── */
    .hero {
      text-align: center;
      padding: 56px 24px 40px;
      max-width: 640px;
      margin: 0 auto;
    }

    .hero-badge {
      display: inline-block;
      background: var(--rose-mid);
      color: var(--rose-dark);
      font-size: 10px;
      letter-spacing: 3px;
      text-transform: uppercase;
      padding: 6px 18px;
      border-radius: 20px;
      margin-bottom: 24px;
      border: 1px solid var(--rose-light);
    }

    .hero h1 {
      font-family: 'Cormorant Garamond', serif;
      font-size: clamp(32px, 6vw, 52px);
      font-weight: 400;
      line-height: 1.2;
      color: var(--text-dark);
      margin-bottom: 20px;
    }

    .hero h1 em {
      font-style: italic;
      color: var(--rose-dark);
    }

    .hero p {
      font-size: 14px;
      line-height: 1.8;
      color: var(--text-mid);
      font-weight: 300;
      max-width: 480px;
      margin: 0 auto;
    }

    /* ── ORNAMENT ── */
    .ornament {
      text-align: center;
      color: var(--rose-light);
      font-size: 22px;
      letter-spacing: 8px;
      margin: 8px 0 32px;
    }

    /* ── FORM CARD ── */
    .form-wrapper {
      max-width: 480px;
      margin: 0 auto 64px;
      padding: 0 24px;
    }

    .form-card {
      background: var(--white);
      border-radius: 20px;
      padding: 40px 36px;
      box-shadow: 0 8px 40px rgba(180, 120, 100, 0.12);
      border: 1px solid var(--rose-light);
    }

    .form-card h2 {
      font-family: 'Cormorant Garamond', serif;
      font-size: 24px;
      font-weight: 400;
      color: var(--text-dark);
      text-align: center;
      margin-bottom: 8px;
    }

    .form-card .form-subtitle {
      font-size: 12px;
      color: var(--text-light);
      text-align: center;
      letter-spacing: 1px;
      margin-bottom: 32px;
    }

    .form-group {
      margin-bottom: 20px;
    }

    .form-group label {
      display: block;
      font-size: 11px;
      letter-spacing: 2px;
      text-transform: uppercase;
      color: var(--text-mid);
      margin-bottom: 8px;
      font-weight: 500;
    }

    .form-group input {
      width: 100%;
      padding: 14px 18px;
      border: 1.5px solid var(--rose-light);
      border-radius: 10px;
      font-family: 'Montserrat', sans-serif;
      font-size: 14px;
      color: var(--text-dark);
      background: var(--rose-bg);
      transition: border-color 0.25s, box-shadow 0.25s;
      outline: none;
    }

    .form-group input::placeholder {
      color: var(--text-light);
      font-weight: 300;
    }

    .form-group input:focus {
      border-color: var(--rose);
      box-shadow: 0 0 0 3px rgba(201, 145, 122, 0.15);
      background: var(--white);
    }

    .btn-submit {
      width: 100%;
      padding: 16px;
      background: linear-gradient(135deg, var(--rose) 0%, var(--rose-dark) 100%);
      color: var(--white);
      border: none;
      border-radius: 10px;
      font-family: 'Montserrat', sans-serif;
      font-size: 13px;
      letter-spacing: 2px;
      text-transform: uppercase;
      font-weight: 500;
      cursor: pointer;
      transition: opacity 0.25s, transform 0.2s;
      margin-top: 8px;
    }

    .btn-submit:hover {
      opacity: 0.9;
      transform: translateY(-1px);
    }

    .btn-submit:active {
      transform: translateY(0);
    }

    .btn-submit:disabled {
      opacity: 0.6;
      cursor: not-allowed;
      transform: none;
    }

    .privacy-note {
      text-align: center;
      font-size: 11px;
      color: var(--text-light);
      margin-top: 16px;
      line-height: 1.6;
    }

    /* ── SUCCESS MESSAGE ── */
    .success-msg {
      display: none;
      text-align: center;
      padding: 16px 0;
    }

    .success-msg .success-icon {
      font-size: 40px;
      margin-bottom: 16px;
    }

    .success-msg h3 {
      font-family: 'Cormorant Garamond', serif;
      font-size: 26px;
      font-weight: 400;
      color: var(--rose-dark);
      margin-bottom: 10px;
    }

    .success-msg p {
      font-size: 13px;
      color: var(--text-mid);
      line-height: 1.7;
    }

    /* ── ERROR MESSAGE ── */
    .error-msg {
      display: none;
      background: #fdecea;
      border: 1px solid #f5c6c2;
      border-radius: 8px;
      padding: 12px 16px;
      font-size: 13px;
      color: #a33;
      text-align: center;
      margin-top: 12px;
    }

    /* ── FOOTER ── */
    footer {
      margin-top: auto;
      text-align: center;
      padding: 24px;
      font-size: 11px;
      color: var(--text-light);
      letter-spacing: 1px;
      border-top: 1px solid var(--rose-light);
    }

    /* ── DECORATIVE DOTS ── */
    .dots-top {
      text-align: center;
      color: var(--rose-light);
      font-size: 8px;
      letter-spacing: 6px;
      margin-bottom: 16px;
    }

    @media (max-width: 480px) {
      .form-card {
        padding: 32px 24px;
      }

      .brand {
        font-size: 38px;
        letter-spacing: 7px;
      }
    }
  </style>
</head>
<body>

  <!-- HEADER -->
  <header>
    <div class="brand-line">
      <span class="brand">Géor</span>
    </div>
    <p class="brand-sub">Prata 925 & Acessórios</p>
  </header>

  <!-- HERO -->
  <section class="hero">
    <span class="hero-badge">✦ Exclusividade & Elegância ✦</span>
    <h1>
      Peças que contam<br/>
      <em>a sua história</em>
    </h1>
    <p>
      Acessórios em prata 925 com acabamento impecável, pensados para quem valoriza o detalhe certo na hora certa.
    </p>
  </section>

  <!-- ORNAMENT -->
  <div class="ornament">· · ·</div>

  <!-- FORM -->
  <div class="form-wrapper">
    <div class="dots-top">✦ ✦ ✦</div>
    <div class="form-card">

      <!-- Form padrão -->
      <div id="form-section">
        <h2>Quero conhecer a Géor</h2>
        <p class="form-subtitle">Preencha abaixo e entraremos em contato</p>

        <form id="leadForm" novalidate>
          <div class="form-group">
            <label for="nome">Seu nome</label>
            <input
              type="text"
              id="nome"
              name="nome"
              placeholder="Como podemos te chamar?"
              autocomplete="given-name"
              required
            />
          </div>

          <div class="form-group">
            <label for="telefone">WhatsApp</label>
            <input
              type="tel"
              id="telefone"
              name="telefone"
              placeholder="(00) 00000-0000"
              autocomplete="tel"
              maxlength="15"
              required
            />
          </div>

          <button type="submit" class="btn-submit" id="submitBtn">
            Quero ser contatada ✦
          </button>

          <div class="error-msg" id="errorMsg">
            Ocorreu um erro. Por favor, tente novamente.
          </div>
        </form>

        <p class="privacy-note">
          Seus dados são confidenciais e não serão compartilhados com terceiros.
        </p>
      </div>

      <!-- Sucesso -->
      <div class="success-msg" id="successMsg">
        <div class="success-icon">✦</div>
        <h3>Que alegria!</h3>
        <p>
          Recebemos seus dados e em breve<br/>
          nossa equipe vai entrar em contato<br/>
          com você pelo WhatsApp.
        </p>
      </div>

    </div>
  </div>

  <!-- FOOTER -->
  <footer>
    © 2026 Géor — Prata 925 & Acessórios
  </footer>

  <script>
    // ── Máscara de telefone ──
    const telInput = document.getElementById('telefone');
    telInput.addEventListener('input', () => {
      let v = telInput.value.replace(/\D/g, '');
      if (v.length > 11) v = v.slice(0, 11);
      if (v.length > 6) {
        v = `(${v.slice(0,2)}) ${v.slice(2,7)}-${v.slice(7)}`;
      } else if (v.length > 2) {
        v = `(${v.slice(0,2)}) ${v.slice(2)}`;
      } else if (v.length > 0) {
        v = `(${v}`;
      }
      telInput.value = v;
    });

    // ── Submit ──
    const form       = document.getElementById('leadForm');
    const submitBtn  = document.getElementById('submitBtn');
    const errorMsg   = document.getElementById('errorMsg');
    const successMsg = document.getElementById('successMsg');
    const formSection = document.getElementById('form-section');

    // ⬇️  Cole aqui a URL gerada pelo Google Apps Script
    const SHEET_URL = 'SUA_URL_DO_APPS_SCRIPT_AQUI';

    form.addEventListener('submit', async (e) => {
      e.preventDefault();
      errorMsg.style.display = 'none';

      const nome     = document.getElementById('nome').value.trim();
      const telefone = telInput.value.trim();

      if (!nome || telefone.replace(/\D/g, '').length < 10) {
        errorMsg.textContent = 'Por favor, preencha nome e WhatsApp corretamente.';
        errorMsg.style.display = 'block';
        return;
      }

      submitBtn.disabled = true;
      submitBtn.textContent = 'Enviando...';

      try {
        await fetch(SHEET_URL, {
          method: 'POST',
          mode: 'no-cors',
          headers: { 'Content-Type': 'application/json' },
          body: JSON.stringify({
            nome,
            telefone,
            data: new Date().toLocaleString('pt-BR')
          })
        });

        // Com no-cors não temos como confirmar erro, assumimos sucesso
        formSection.style.display = 'none';
        successMsg.style.display  = 'block';

      } catch (err) {
        errorMsg.textContent = 'Ocorreu um erro. Por favor, tente novamente.';
        errorMsg.style.display = 'block';
        submitBtn.disabled = false;
        submitBtn.textContent = 'Quero ser contatada ✦';
      }
    });
  </script>

</body>
</html>
