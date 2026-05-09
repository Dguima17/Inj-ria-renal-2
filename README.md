<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Injúria Renal Aguda – Guia Completo</title>
<link href="[https://fonts.googleapis.com/css2?family=Playfair+Display:wght@700;900&family=Source+Sans+3:wght@300;400;600&display=swap](https://fonts.googleapis.com/css2?family=Playfair+Display:wght@700;900&family=Source+Sans+3:wght@300;400;600&display=swap)" rel="stylesheet">
<style>
  :root {
    --kidney: #c0392b;
    --kidney-light: #e74c3c;
    --kidney-dark: #922b21;
    --gold: #d4a017;
    --teal: #1a6b6b;
    --teal-light: #2e9e9e;
    --navy: #0f2744;
    --cream: #fdf6ec;
    --text: #1a1a2e;
    --muted: #5a6a7a;
    --bg: #f4f0eb;
  }

  * { box-sizing: border-box; margin: 0; padding: 0; }

  body {
    font-family: 'Source Sans 3', sans-serif;
    background: var(--bg);
    color: var(--text);
    line-height: 1.7;
  }

  header {
    background: var(--navy);
    color: white;
    padding: 3rem 2rem 2rem;
    text-align: center;
    position: relative;
    overflow: hidden;
  }
  header .tag {
    display: inline-block;
    background: var(--kidney);
    color: white;
    font-size: 0.75rem;
    font-weight: 600;
    letter-spacing: 2px;
    text-transform: uppercase;
    padding: 4px 14px;
    border-radius: 20px;
    margin-bottom: 1rem;
  }
  header h1 {
    font-family: 'Playfair Display', serif;
    font-size: clamp(2rem, 5vw, 3.4rem);
    font-weight: 900;
    line-height: 1.15;
    margin-bottom: 0.5rem;
  }
  header p {
    color: rgba(255,255,255,0.65);
    font-size: 0.95rem;
  }

  nav {
    background: var(--kidney-dark);
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    position: sticky;
    top: 0;
    z-index: 100;
    box-shadow: 0 2px 8px rgba(0,0,0,0.25);
  }
  nav a {
    color: white;
    text-decoration: none;
    padding: 0.7rem 1.1rem;
    font-size: 0.82rem;
    font-weight: 600;
    text-transform: uppercase;
  }
  nav a:hover { background: var(--kidney-light); }

  main { max-width: 960px; margin: 0 auto; padding: 2rem 1.2rem 4rem; }

  section {
    background: white;
    border-radius: 12px;
    margin-bottom: 2rem;
    overflow: hidden;
    box-shadow: 0 2px 12px rgba(0,0,0,0.07);
  }

  .sec-header {
    display: flex;
    align-items: center;
    gap: 1rem;
    padding: 1.2rem 1.6rem;
    cursor: pointer;
    background: #fff;
  }
  .sec-header:hover { background: #fdf0ee; }
  .sec-number {
    font-family: 'Playfair Display', serif;
    font-size: 2rem;
    font-weight: 900;
    color: var(--kidney);
  }
  .sec-title {
    font-family: 'Playfair Display', serif;
    font-size: 1.25rem;
    font-weight: 700;
    color: var(--navy);
    flex: 1;
  }
  .sec-arrow { transition: transform 0.3s; color: var(--kidney); }
  .sec-header.open .sec-arrow { transform: rotate(180deg); }

  .sec-body {
    padding: 0 1.6rem;
    display: none;
  }
  .sec-body.open {
    display: block;
    padding: 0 1.6rem 1.6rem;
  }

  h3 {
    font-family: 'Playfair Display', serif;
    font-size: 1.1rem;
    color: var(--kidney-dark);
    margin: 1.5rem 0 0.5rem;
    border-left: 3px solid var(--kidney);
    padding-left: 0.7rem;
  }

  .grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 1rem; margin: 1rem 0; }
  .card { background: var(--cream); border-radius: 8px; padding: 1rem; border-top: 4px solid var(--kidney); }
  
  .alert { border-radius: 8px; padding: 1rem; margin: 1rem 0; font-weight: 600; }
  .alert.teal { background: #e6f4f4; color: #1a6b6b; border-left: 4px solid #1a6b6b; }
  .alert.gold { background: #fef9e7; color: #7d6008; border-left: 4px solid #d4a017; }
  .alert.navy { background: #eaf0f8; color: #0f2744; border-left: 4px solid #0f2744; }
  .alert.red { background: #fde8e6; color: #922b21; border-left: 4px solid #c0392b; }

  table { width: 100%; border-collapse: collapse; margin: 1rem 0; font-size: 0.9rem; }
  th { background: var(--kidney); color: white; padding: 0.7rem; text-align: left; }
  td { padding: 0.7rem; border-bottom: 1px solid #eee; }

  .pill { display: inline-block; background: var(--kidney); color: white; border-radius: 20px; padding: 2px 10px; font-size: 0.8rem; margin: 2px; }

  footer { text-align: center; padding: 2rem; color: var(--muted); border-top: 1px solid #ddd; }
</style>
</head>
<body>

<header>
  <div class="tag">Nefrologia · FAMETRO 7º Período</div>
  <h1>Injúria Renal Aguda</h1>
  <p>Daniel Guimarães · Guia Completo de Estudo</p>
</header>

<nav>
  <a href="#s1">Definição</a>
  <a href="#s3">Critérios</a>
  <a href="#s5">Diagnóstico</a>
  <a href="#s6">Causas</a>
  <a href="#s10">Diálise</a>
</nav>

<main>
  <!-- 1 DEFINIÇÃO -->
  <section id="s1">
    <div class="sec-header open" onclick="toggle(this)">
      <span class="sec-number">01</span>
      <span class="sec-title">Definição de IRA (AKI)</span>
      <span class="sec-arrow">▼</span>
    </div>
    <div class="sec-body open">
      <div class="alert teal">💡 IRA = diminuição abrupta da função renal → retenção de produtos nitrogenados + desequilíbrio eletrolítico.</div>
      <h3>Critérios KDIGO 2012</h3>
      <div class="grid">
        <div class="card"><strong>Critério 1</strong><span>↑ Creatinina ≥ 0,3 mg/dL em 48h</span></div>
        <div class="card"><strong>Critério 2</strong><span>↑ Creatinina ≥ 1,5× basal em 7 dias</span></div>
        <div class="card"><strong>Critério 3</strong><span>Débito urinário < 0,5 mL/kg/h por ≥ 6h</span></div>
      </div>
    </div>
  </section>

  <!-- 3 ESTADIAMENTO -->
  <section id="s3">
    <div class="sec-header" onclick="toggle(this)">
      <span class="sec-number">03</span>
      <span class="sec-title">Estadiamento KDIGO</span>
      <span class="sec-arrow">▼</span>
    </div>
    <div class="sec-body">
      <table>
        <thead><tr><th>Estágio</th><th>Creatinina</th><th>Diurese</th></tr></thead>
        <tbody>
          <tr><td><span class="pill">1</span></td><td>1,5–1,9× basal</td><td>< 0,5 mL/kg/h (6-12h)</td></tr>
          <tr><td><span class="pill">2</span></td><td>2,0–2,9× basal</td><td>< 0,5 mL/kg/h (>12h)</td></tr>
          <tr><td><span class="pill">3</span></td><td>≥ 3× basal ou Cr ≥ 4</td><td>< 0,3 mL/kg/h (>24h)</td></tr>
        </tbody>
      </table>
    </div>
  </section>

  <!-- 10 DIÁLISE -->
  <section id="s10">
    <div class="sec-header" onclick="toggle(this)">
      <span class="sec-number">10</span>
      <span class="sec-title">Indicações de Diálise (AEIOU)</span>
      <span class="sec-arrow">▼</span>
    </div>
    <div class="sec-body">
      <div class="alert navy">
        <p><strong>A</strong>cidose Refratária (pH < 7,1)</p>
        <p><strong>E</strong>letrólitos (K+ > 6,5)</p>
        <p><strong>I</strong>ntoxicações Dialisáveis</p>
        <p><strong>O</strong>verload (Congestão Refratária)</p>
        <p><strong>U</strong>remia (Encefalopatia/Pericardite)</p>
      </div>
    </div>
  </section>

  <!-- QUESTÃO -->
  <section>
    <div class="sec-header" onclick="toggle(this)">
      <span class="sec-number">🎓</span>
      <span class="sec-title">Questão UNICAMP 2022</span>
      <span class="sec-arrow">▼</span>
    </div>
    <div class="sec-body">
      <p>Homem, 72 anos, ↓ diurese pós-cateterismo. Livedo reticular + Eosinofilia.</p>
      <div class="alert teal">✅ Resposta: Doença Ateroembólica</div>
    </div>
  </section>
</main>

<footer>
  Daniel Guimarães — FAMETRO 7º Período · Nefrologia
</footer>

<script>
function toggle(header) {
  header.classList.toggle('open');
  const body = header.nextElementSibling;
  body.classList.toggle('open');
}
</script>

</body>
</html>
