<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Jeremías Salomón Rosa</title>
<link href="https://fonts.googleapis.com/css2?family=Fira+Code:wght@400;500;600&family=Newsreader:ital,wght@0,300;0,400;0,600;1,300&display=swap" rel="stylesheet">
<style>
  :root {
    --bg: #f5f2eb;
    --paper: #faf8f3;
    --ink: #1a1814;
    --ink-light: #5a5650;
    --accent: #c0392b;
    --rule: #c8c0b0;
    --code-bg: #ede9e0;
    --mono: 'Fira Code', monospace;
    --serif: 'Newsreader', Georgia, serif;
  }
 
  * { box-sizing: border-box; margin: 0; padding: 0; }
  html { scroll-behavior: smooth; }
 
  body {
    background: var(--bg);
    color: var(--ink);
    font-family: var(--serif);
    font-size: 18px;
    line-height: 1.75;
    padding: 0 16px 60px;
  }
 
  .page {
    max-width: 760px;
    margin: 0 auto;
    background: var(--paper);
    border-left: 1px solid var(--rule);
    border-right: 1px solid var(--rule);
    padding: 56px 64px 72px;
    position: relative;
    box-shadow: 0 2px 40px rgba(0,0,0,0.06);
  }
 
  @media (max-width: 600px) {
    .page { padding: 36px 24px 52px; }
    body { font-size: 16px; }
  }
 
  .page::before {
    content: '1\A 2\A 3\A 4\A 5\A 6\A 7\A 8\A 9\A10\A11\A12\A13\A14\A15\A16\A17\A18\A19\A20\A21\A22\A23\A24\A25\A26\A27\A28\A29\A30\A31\A32\A33\A34\A35\A36\A37\A38\A39\A40';
    white-space: pre;
    position: absolute;
    left: 0; top: 56px;
    width: 44px;
    text-align: right;
    padding-right: 12px;
    font-family: var(--mono);
    font-size: 0.65rem;
    color: #c0b8a8;
    line-height: 2.15rem;
    pointer-events: none;
    user-select: none;
  }
 
  h1 {
    font-family: var(--mono);
    font-size: clamp(1.15rem, 3vw, 1.45rem);
    font-weight: 600;
    color: var(--ink);
    margin-bottom: 6px;
    letter-spacing: -0.01em;
  }
  h1 .hash { color: var(--accent); margin-right: 6px; }
  h1 .emoji { font-style: normal; }
 
  .md-hr {
    font-family: var(--mono);
    color: var(--rule);
    font-size: 0.85rem;
    margin: 18px 0;
    letter-spacing: 0.08em;
    user-select: none;
  }
  .md-hr-thick { color: #a09888; }
 
  h2 {
    font-family: var(--mono);
    font-size: clamp(1rem, 2.5vw, 1.2rem);
    font-weight: 600;
    color: var(--ink);
    margin-bottom: 14px;
  }
  h2 .hash { color: var(--accent); margin-right: 4px; }
 
  .body-text {
    font-family: var(--serif);
    font-size: clamp(0.95rem, 2vw, 1.05rem);
    color: #3a3630;
    line-height: 1.85;
    font-weight: 300;
    font-style: italic;
    padding-left: 20px;
    border-left: 2px solid var(--rule);
    margin-bottom: 4px;
  }
  .body-text .hash { font-family: var(--mono); color: var(--accent); font-size: 0.9em; font-style: normal; margin-right: 4px; }
 
  .tech-line {
    font-family: var(--mono);
    font-size: 0.78rem;
    padding-left: 20px;
    border-left: 2px solid var(--rule);
    display: flex; flex-wrap: wrap; gap: 10px; align-items: center;
  }
  .tech-line .hash { color: var(--accent); margin-right: 4px; }
 
  .pill {
    display: inline-flex; align-items: center; gap: 6px;
    background: var(--code-bg);
    border: 1px solid var(--rule);
    border-radius: 5px;
    padding: 4px 12px;
    font-size: 0.78rem;
    color: var(--ink);
    text-decoration: none;
    transition: all 0.2s ease;
    cursor: pointer;
    font-family: var(--mono);
  }
  .pill:hover {
    background: var(--ink);
    color: #f5f2eb;
    border-color: var(--ink);
    transform: translateY(-1px);
  }
  .pill .dot { width: 7px; height: 7px; border-radius: 50%; flex-shrink: 0; }
 
  .contact-line {
    font-family: var(--mono);
    font-size: 0.82rem;
    padding-left: 20px;
    border-left: 2px solid var(--rule);
    display: flex; align-items: center; gap: 10px; flex-wrap: wrap;
  }
  .contact-line .hash { color: var(--accent); }
  .contact-line a {
    color: var(--accent);
    text-decoration: none;
    border-bottom: 1px solid transparent;
    transition: border-color 0.2s;
  }
  .contact-line a:hover { border-color: var(--accent); }
 
  .cursor {
    display: inline-block;
    width: 10px; height: 1.1em;
    background: var(--accent);
    vertical-align: text-bottom;
    margin-left: 4px;
    animation: blink 1s step-end infinite;
  }
  @keyframes blink { 0%,100%{opacity:1} 50%{opacity:0} }
 
  .toolbar {
    display: flex; align-items: center; gap: 8px;
    padding: 12px 20px;
    background: #ede9e0;
    border-bottom: 1px solid var(--rule);
    margin: -56px -64px 40px;
  }
  @media (max-width: 600px) {
    .toolbar { margin: -36px -24px 32px; }
  }
  .dot-r { width: 12px; height: 12px; border-radius: 50%; background: #e74c3c; }
  .dot-y { width: 12px; height: 12px; border-radius: 50%; background: #f1c40f; }
  .dot-g { width: 12px; height: 12px; border-radius: 50%; background: #2ecc71; }
  .toolbar-title {
    font-family: var(--mono);
    font-size: 0.72rem;
    color: #908880;
    margin-left: auto; margin-right: auto;
    letter-spacing: 0.05em;
  }
 
  .spacer { height: 24px; }
  .spacer-sm { height: 12px; }
</style>
</head>
<body>
<div class="page">
 
  <div class="toolbar">
    <div class="dot-r"></div>
    <div class="dot-y"></div>
    <div class="dot-g"></div>
    <span class="toolbar-title">portafolio.md</span>
  </div>
 
  <h1><span class="hash">#</span> ¡Hola! Soy Jeremías Salomón Rosa <span class="emoji">👋</span></h1>
 
  <div class="md-hr">---</div>
 
  <h2><span class="hash">##</span> Sobre mí:</h2>
 
  <div class="md-hr">---</div>
 
  <p class="body-text">
    <span class="hash">###</span>
    Soy docente en Informática y licenciado en la Enseñanza de la Matemática con más de 10 años de experiencia en la docencia. Actualmente estoy en proceso de formación en el <strong>Curso Transformación Digital para la Docencia Técnica 1</strong>, donde las expectativas son grandes principalmente en adquirir nuevos aprendizajes y actualizarme, con la mentalidad de aprender nuevas herramientas para poder aplicarlas en el aula.
  </p>
 
  <div class="md-hr md-hr-thick spacer-sm">___</div>
  <div class="spacer-sm"></div>
 
  <h2><span class="hash">##</span> Tecnologías:</h2>
  <div class="spacer-sm"></div>
 
  <div class="tech-line">
    <span class="hash">###</span>
    <a class="pill" href="https://developer.mozilla.org/es/docs/Web/HTML" target="_blank">
      <span class="dot" style="background:#e34c26"></span>HTML5
    </a>
    <a class="pill" href="https://developer.mozilla.org/es/docs/Web/CSS" target="_blank">
      <span class="dot" style="background:#264de4"></span>CSS3
    </a>
    <a class="pill" href="https://www.php.net" target="_blank">
      <span class="dot" style="background:#8993be"></span>PHP
    </a>
    <a class="pill" href="https://www.mysql.com" target="_blank">
      <span class="dot" style="background:#00758f"></span>MySQL
    </a>
    <a class="pill" href="https://developer.mozilla.org/es/docs/Web/JavaScript" target="_blank">
      <span class="dot" style="background:#f7df1e"></span>JavaScript
    </a>
    <a class="pill" href="https://www.python.org" target="_blank">
      <span class="dot" style="background:#3776ab"></span>Python
    </a>
    <a class="pill" href="https://code.visualstudio.com" target="_blank">
      <span class="dot" style="background:#007acc"></span>VSCode
    </a>
  </div>
 
  <div class="md-hr md-hr-thick spacer-sm" style="margin-top:20px">___</div>
  <div class="spacer-sm"></div>
 
  <h2><span class="hash">##</span> Contacto:</h2>
  <div class="spacer-sm"></div>
 
  <div class="contact-line">
    <span class="hash">###</span>
    <span>E-Mail:</span>
    <a href="mailto:jeremiassrosapassasin@gmail.com">jeremiassrosapassasin@gmail.com</a>
  </div>
 
  <span class="cursor"></span>
 
</div>
</body>
</html>
