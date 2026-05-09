<!DOCTYPE html>

<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Injúria Renal Aguda – Guia Completo</title>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@700;900&family=Source+Sans+3:wght@300;400;600&display=swap" rel="stylesheet">
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

- { box-sizing: border-box; margin: 0; padding: 0; }

body {
font-family: ‘Source Sans 3’, sans-serif;
background: var(–bg);
color: var(–text);
line-height: 1.7;
}

/* HEADER */
header {
background: var(–navy);
color: white;
padding: 3rem 2rem 2rem;
text-align: center;
position: relative;
overflow: hidden;
}
header::before {
content: ‘’;
position: absolute;
top: -60px; left: -60px;
width: 220px; height: 220px;
border-radius: 50%;
background: rgba(192,57,43,0.18);
}
header::after {
content: ‘’;
position: absolute;
bottom: -40px; right: -40px;
width: 160px; height: 160px;
border-radius: 50%;
background: rgba(26,107,107,0.2);
}
header .tag {
display: inline-block;
background: var(–kidney);
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
font-family: ‘Playfair Display’, serif;
font-size: clamp(2rem, 5vw, 3.4rem);
font-weight: 900;
line-height: 1.15;
margin-bottom: 0.5rem;
}
header p {
color: rgba(255,255,255,0.65);
font-size: 0.95rem;
letter-spacing: 0.5px;
}

/* NAV */
nav {
background: var(–kidney-dark);
display: flex;
flex-wrap: wrap;
justify-content: center;
gap: 0;
position: sticky;
top: 0;
z-index: 100;
box-shadow: 0 2px 8px rgba(0,0,0,0.25);
}
nav a {
color: rgba(255,255,255,0.85);
text-decoration: none;
padding: 0.7rem 1.1rem;
font-size: 0.82rem;
font-weight: 600;
letter-spacing: 0.5px;
text-transform: uppercase;
transition: background 0.2s, color 0.2s;
}
nav a:hover { background: var(–kidney-light); color: white; }

/* MAIN */
main { max-width: 960px; margin: 0 auto; padding: 2rem 1.2rem 4rem; }

/* SECTION */
section {
background: white;
border-radius: 12px;
margin-bottom: 2rem;
overflow: hidden;
box-shadow: 0 2px 12px rgba(0,0,0,0.07);
animation: fadeUp 0.5s ease both;
}
@keyframes fadeUp {
from { opacity: 0; transform: translateY(18px); }
to   { opacity: 1; transform: translateY(0); }
}

.sec-header {
display: flex;
align-items: center;
gap: 1rem;
padding: 1.2rem 1.6rem;
cursor: pointer;
user-select: none;
transition: background 0.2s;
}
.sec-header:hover { background: #fdf0ee; }
.sec-number {
font-family: ‘Playfair Display’, serif;
font-size: 2rem;
font-weight: 900;
color: var(–kidney);
line-height: 1;
min-width: 2.2rem;
}
.sec-title {
font-family: ‘Playfair Display’, serif;
font-size: 1.25rem;
font-weight: 700;
color: var(–navy);
flex: 1;
}
.sec-arrow {
font-size: 1rem;
color: var(–kidney);
transition: transform 0.3s;
}
.sec-header.open .sec-arrow { transform: rotate(180deg); }

.sec-body {
padding: 0 1.6rem;
max-height: 0;
overflow: hidden;
transition: max-height 0.5s ease, padding 0.3s;
}
.sec-body.open {
max-height: 9000px;
padding: 0 1.6rem 1.6rem;
}

/* DIVIDER */
.divider {
height: 3px;
background: linear-gradient(90deg, var(–kidney), var(–teal));
border-radius: 2px;
margin: 1.2rem 0;
}

/* SUBSECTIONS */
h3 {
font-family: ‘Playfair Display’, serif;
font-size: 1.05rem;
font-weight: 700;
color: var(–kidney-dark);
margin: 1.4rem 0 0.5rem;
border-left: 3px solid var(–kidney);
padding-left: 0.7rem;
}
h4 {
font-size: 0.95rem;
font-weight: 600;
color: var(–teal);
margin: 1rem 0 0.3rem;
}
p { margin-bottom: 0.7rem; font-size: 0.97rem; color: #333; }

/* CARDS GRID */
.grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(220px,1fr)); gap: 1rem; margin: 1rem 0; }
.card {
background: var(–cream);
border-radius: 8px;
padding: 1rem 1.1rem;
border-top: 4px solid var(–kidney);
}
.card.teal { border-top-color: var(–teal); }
.card.gold  { border-top-color: var(–gold); }
.card.navy  { border-top-color: var(–navy); }
.card strong {
display: block;
font-size: 0.85rem;
text-transform: uppercase;
letter-spacing: 0.5px;
color: var(–muted);
margin-bottom: 0.3rem;
}
.card span { font-size: 0.95rem; color: var(–text); }

/* TABLE */
.tbl-wrap { overflow-x: auto; margin: 1rem 0; }
table { width: 100%; border-collapse: collapse; font-size: 0.9rem; }
thead tr { background: var(–kidney); color: white; }
th, td { padding: 0.6rem 0.9rem; text-align: left; border-bottom: 1px solid #eee; }
tbody tr:nth-child(even) { background: #fdf6ec; }
tbody tr:hover { background: #fce4e1; }

/* ALERT BOX */
.alert {
border-radius: 8px;
padding: 0.85rem 1.1rem;
margin: 0.8rem 0;
font-size: 0.93rem;
font-weight: 600;
display: flex;
gap: 0.6rem;
align-items: flex-start;
}
.alert.red   { background: #fde8e6; color: #922b21; border-left: 4px solid #c0392b; }
.alert.teal  { background: #e6f4f4; color: #1a6b6b; border-left: 4px solid #1a6b6b; }
.alert.gold  { background: #fef9e7; color: #7d6008; border-left: 4px solid #d4a017; }
.alert.navy  { background: #eaf0f8; color: #0f2744; border-left: 4px solid #0f2744; }

/* LIST */
ul, ol { padding-left: 1.4rem; margin-bottom: 0.7rem; }
li { margin-bottom: 0.3rem; font-size: 0.96rem; }

/* PILL */
.pill {
display: inline-block;
background: var(–kidney);
color: white;
border-radius: 20px;
padding: 2px 12px;
font-size: 0.78rem;
font-weight: 600;
margin: 2px 2px;
}
.pill.teal  { background: var(–teal); }
.pill.navy  { background: var(–navy); }
.pill.gold  { background: var(–gold); color: #333; }

/* HIGHLIGHT */
mark { background: #ffeaa0; border-radius: 3px; padding: 0 3px; }

/* FLOW */
.flow {
display: flex;
align-items: center;
gap: 0.5rem;
flex-wrap: wrap;
margin: 0.8rem 0;
}
.flow-step {
background: var(–navy);
color: white;
border-radius: 6px;
padding: 0.4rem 0.9rem;
font-size: 0.85rem;
font-weight: 600;
}
.flow-arrow { color: var(–kidney); font-size: 1.2rem; font-weight: 700; }

/* MNEMONIC */
.mnemonic {
background: var(–navy);
color: white;
border-radius: 10px;
padding: 1rem 1.3rem;
margin: 1rem 0;
}
.mnemonic .letra {
font-family: ‘Playfair Display’, serif;
font-size: 1.6rem;
font-weight: 900;
color: var(–gold);
}
.mnemonic p { color: rgba(255,255,255,0.85); margin: 0; font-size: 0.93rem; }

/* FOOTER */
footer {
text-align: center;
padding: 2rem;
color: var(–muted);
font-size: 0.82rem;
border-top: 1px solid #ddd;
margin-top: 2rem;
}

@media (max-width: 600px) {
nav a { padding: 0.6rem 0.7rem; font-size: 0.72rem; }
.sec-title { font-size: 1.05rem; }
}
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
  <a href="#s2">Histórico</a>
  <a href="#s3">Critérios</a>
  <a href="#s4">Epidemiologia</a>
  <a href="#s5">Diagnóstico</a>
  <a href="#s6">Causas</a>
  <a href="#s7">Fisiopatologia</a>
  <a href="#s8">Evolução</a>
  <a href="#s9">Tratamento</a>
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
    <div class="alert teal">💡 IRA = diminuição abrupta da função renal → retenção de produtos nitrogenados + desequilíbrio eletrolítico e do volume extracelular, com ou sem oligúria.</div>

```
<h3>Critérios KDIGO 2012 (qualquer um dos seguintes)</h3>
<div class="grid">
  <div class="card">
    <strong>Critério 1</strong>
    <span>↑ Creatinina ≥ 0,3 mg/dL em <mark>48 horas</mark></span>
  </div>
  <div class="card teal">
    <strong>Critério 2</strong>
    <span>↑ Creatinina ≥ 1,5× basal nos últimos <mark>7 dias</mark></span>
  </div>
  <div class="card gold">
    <strong>Critério 3</strong>
    <span>Débito urinário &lt; 0,5 mL/kg/h por <mark>≥ 6 horas</mark></span>
  </div>
</div>

<h3>Novidades KDIGO 2026 (rascunho público)</h3>
<p>A nova diretriz adiciona <strong>critérios estruturais</strong> além dos funcionais:</p>
<ul>
  <li>↑ Cistatina C ≥ 1,5× basal nos últimos 7 dias</li>
  <li>Elevação de biomarker de dano renal validado nos últimos 7 dias</li>
  <li>Volume urinário médio &lt; 0,5 mL/kg/h (peso ideal) por ≥ 6 h</li>
</ul>
<div class="alert gold">⚠️ A Cistatina C agora é recomendada (2B) para identificar IRA em situações onde a creatinina é menos precisa (ex.: amputados, desnutridos).</div>
```

  </div>
</section>

<!-- 2 HISTÓRICO -->

<section id="s2">
  <div class="sec-header" onclick="toggle(this)">
    <span class="sec-number">02</span>
    <span class="sec-title">Histórico — Crush Syndrome (Bywaters, 1940)</span>
    <span class="sec-arrow">▼</span>
  </div>
  <div class="sec-body">
    <p>A primeira descrição formal do que hoje chamamos de IRA surgiu durante a <strong>2ª Guerra Mundial</strong>, no Blitz de Londres (1940), pelo Dr. E.G.L. Bywaters no Hammersmith Hospital.</p>
    <div class="flow">
      <div class="flow-step">Vítima soterrada por horas</div>
      <span class="flow-arrow">→</span>
      <div class="flow-step">Aparentemente ilesa ao resgate</div>
      <span class="flow-arrow">→</span>
      <div class="flow-step">Colapso súbito + edema de membros</div>
      <span class="flow-arrow">→</span>
      <div class="flow-step">Oligúria → Uremia → Morte</div>
    </div>
    <h3>Mecanismo descoberto</h3>
    <ul>
      <li><strong>Rabdomiólise</strong>: necrose muscular libera <strong>mioglobina</strong></li>
      <li>Mioglobina é nefrotóxica → obstrução dos túbulos renais</li>
      <li>Analogia com transfusão incompatível (Baker & Dodds, 1925)</li>
    </ul>
    <div class="alert navy">📚 Essa é a <strong>1ª descrição da "Insuficiência Renal Aguda"</strong> na literatura médica.</div>
  </div>
</section>

<!-- 3 CRITÉRIOS E ESTADIAMENTO -->

<section id="s3">
  <div class="sec-header" onclick="toggle(this)">
    <span class="sec-number">03</span>
    <span class="sec-title">Estadiamento — RIFLE vs AKIN vs KDIGO</span>
    <span class="sec-arrow">▼</span>
  </div>
  <div class="sec-body">

```
<h3>RIFLE (2004)</h3>
<div class="tbl-wrap">
  <table>
    <thead><tr><th>Estágio</th><th>Creatinina / TFG</th><th>Diurese</th></tr></thead>
    <tbody>
      <tr><td><span class="pill">R – Risco</span></td><td>Cr ×1,5 ou TFG ↓ 25%</td><td>&lt;0,5 mL/kg/h × 6h</td></tr>
      <tr><td><span class="pill">I – Injúria</span></td><td>Cr ×2 ou TFG ↓ 50%</td><td>&lt;0,5 mL/kg/h × 12h</td></tr>
      <tr><td><span class="pill">F – Falência</span></td><td>Cr ×3 / ≥4 mg/dL ou TFG ↓ 75%</td><td>&lt;0,3 mL/kg/h × 24h ou anúria × 12h</td></tr>
      <tr><td><span class="pill navy">L – Perda</span></td><td colspan="2">Perda completa &gt; 4 semanas</td></tr>
      <tr><td><span class="pill navy">E – ESRD</span></td><td colspan="2">Doença renal terminal</td></tr>
    </tbody>
  </table>
</div>

<h3>KDIGO 2012 — Estadiamento (ainda vigente)</h3>
<div class="tbl-wrap">
  <table>
    <thead><tr><th>Estágio</th><th>Creatinina sérica</th><th>Diurese</th></tr></thead>
    <tbody>
      <tr><td><span class="pill gold" style="color:#333">1</span></td><td>1,5–1,9× basal <em>ou</em> ↑ ≥0,3 mg/dL</td><td>&lt;0,5 mL/kg/h por 6–12h</td></tr>
      <tr><td><span class="pill" style="background:#e67e22">2</span></td><td>2,0–2,9× basal</td><td>&lt;0,5 mL/kg/h por ≥12h</td></tr>
      <tr><td><span class="pill">3</span></td><td>≥3× basal <em>ou</em> Cr ≥4 mg/dL <em>ou</em> início de TRS</td><td>&lt;0,3 mL/kg/h por ≥24h <em>ou</em> anúria ≥12h</td></tr>
    </tbody>
  </table>
</div>

<div class="alert red">🔴 Pacientes que preenchem critério de <strong>creatinina E débito urinário</strong> têm pior prognóstico! AKI 3 (Cr) + AKI 1 (DU) → mortalidade 38%; AKI 3 + DU ↓↓ → mortalidade 51,1%.</div>

<h3>Novo estadiamento KDIGO 2026</h3>
<p>Incorpora <strong>3 dimensões independentes</strong> (C, U, B):</p>
<ul>
  <li><strong>C0–C3</strong>: estadio pela creatinina sérica</li>
  <li><strong>U0–U3</strong>: estadio pelo débito urinário</li>
  <li><strong>B0 / B1</strong>: ausência ou presença de biomarker de dano positivo</li>
</ul>
```

  </div>
</section>

<!-- 4 EPIDEMIOLOGIA -->

<section id="s4">
  <div class="sec-header" onclick="toggle(this)">
    <span class="sec-number">04</span>
    <span class="sec-title">Importância & Epidemiologia</span>
    <span class="sec-arrow">▼</span>
  </div>
  <div class="sec-body">
    <div class="alert red">⚠️ IRA em UTI é fator de risco independente para óbito. Mortalidade quando necessita Suporte Renal Artificial (SRA): <strong>40–55%</strong>!</div>

```
<h3>Taxas de mortalidade por contexto</h3>
<div class="grid">
  <div class="card"><strong>AKI com SRA</strong><span>40–55%</span></div>
  <div class="card teal"><strong>Sepse sem AKI</strong><span>15–25%</span></div>
  <div class="card gold"><strong>IAM</strong><span>~20%</span></div>
  <div class="card navy"><strong>SARA + VMI</strong><span>30–40%</span></div>
</div>

<h3>Epidemiologia por população (UTI adultos)</h3>
<div class="tbl-wrap">
  <table>
    <thead><tr><th>População</th><th>Incidência</th><th>Diálise (%)</th><th>Mortalidade (%)</th></tr></thead>
    <tbody>
      <tr><td>Hospitalizados adultos</td><td>1 em 5 (20%)</td><td>&lt;10</td><td>10–20</td></tr>
      <tr><td>UTI adultos</td><td>1/3 a 2/3 (30–60%)</td><td>5–11</td><td>20–50</td></tr>
      <tr><td>Cirurgia cardíaca adultos</td><td>1/5 (2–50%)</td><td>&lt;5</td><td>10</td></tr>
      <tr><td>Sepse adultos</td><td>1/20 a 1/2 (5–50%)</td><td>15</td><td>30–60</td></tr>
    </tbody>
  </table>
</div>

<h3>Rede Latino-Americana de IRA (2004)</h3>
<ul>
  <li>2.479 pacientes / 19 unidades</li>
  <li>63,8% em UTI (sepse e choque como principais causas)</li>
  <li>Mortalidade geral: <strong>32,3%</strong></li>
  <li>Incidência aumenta com a idade</li>
</ul>

<h3>Creatinina × Mortalidade (pós cirurgia cardíaca)</h3>
<p>Aumentos progressivos da creatinina no pós-operatório se associam a aumentos exponenciais da mortalidade em 30 dias.</p>
<div class="alert teal">📊 Aumentos de Cr ≥ 0,3 mg/dL associam-se independentemente a <strong>4× aumento na mortalidade hospitalar</strong> (Chertow et al., JASN 2005).</div>
```

  </div>
</section>

<!-- 5 DIAGNÓSTICO -->

<section id="s5">
  <div class="sec-header" onclick="toggle(this)">
    <span class="sec-number">05</span>
    <span class="sec-title">Diagnóstico — Marcadores e Exames</span>
    <span class="sec-arrow">▼</span>
  </div>
  <div class="sec-body">

```
<h3>🏆 Creatinina Sérica — "Carro-Chefe"</h3>
<p>Produzida a partir da <strong>creatina muscular</strong> (Arg + Glyc → fígado → músculo). Filtrada livremente pelo glomérulo; ~10% secretada no TCP.</p>
<h4>Fatores que interferem (podem subestimar ou superestimar a função renal)</h4>
<ul>
  <li>↑ falsamente: suplementação de creatina, dieta hiperproteica, infecções (catabolismo)</li>
  <li>↓ falsamente: amputação, desnutrição, veganos, doença hepática, edema (dilui)</li>
  <li>Drogas que ↑ Cr sem alterar TFG: <strong>Trimetoprima, Dolutegravir</strong></li>
</ul>
<div class="alert red">⛔ Relação Cr × TFG é <strong>não linear</strong>. A Cr sobe em média 1 mg/dL/dia na anúria — fica dias atrasada em relação ao dano real!</div>

<h3>Ureia — "Robin" (secundária)</h3>
<p>Valor normal: 20–30 mg/dL. Formada no fígado a partir da amônia.</p>
<h4>Causas de ↑ ureia SEM alteração da TFG</h4>
<ul>
  <li>Hemorragia digestiva alta</li>
  <li>Corticoides</li>
  <li>Dieta hiperproteica</li>
  <li>Depleção de volume intravascular ("IRA pré-renal")</li>
  <li>Estados hipercatabólicos</li>
</ul>
<div class="alert gold">📌 Relação Ureia/Creatinina &gt; 40 → pensar em <strong>hemorragia digestiva alta</strong> ou uso de corticoides!</div>

<h3>Cistatina C — Melhor marcador de TFG</h3>
<ul>
  <li>Proteína de 13,36 kDa — filtrada livremente, reabsorvida e metabolizada no TCP</li>
  <li><strong>Não afetada</strong> por sexo, raça ou massa muscular</li>
  <li>Ideal para: <mark>amputados, desnutridos, crianças, idosos</mark></li>
  <li>Afetada por: corticoides em excesso, distúrbios de tireoide, tabagismo</li>
  <li>KDIGO 2026: recomenda seu uso (2B) quando Cr é menos precisa</li>
</ul>

<h3>Clearance de Creatinina — Fórmulas</h3>
<div class="tbl-wrap">
  <table>
    <thead><tr><th>Fórmula</th><th>Uso</th></tr></thead>
    <tbody>
      <tr><td><strong>Cockroft-Gault</strong></td><td>(140-idade × peso)/72 × Cr × (0,85 se mulher) — usada para ajuste de doses de drogas</td></tr>
      <tr><td><strong>MDRD simplificada</strong></td><td>186 × Cr⁻¹,¹⁵⁴ × idade⁻⁰,²⁰³ × (0,742 se mulher)</td></tr>
      <tr><td><strong>CKD-EPI</strong></td><td>Mais usada atualmente — mais precisa em TFG &gt; 60</td></tr>
    </tbody>
  </table>
</div>

<h3>Estudos Urinários</h3>
<h4>Fluxo Urinário</h4>
<ul>
  <li>Oligúria: DU &lt; 0,5 mL/kg/h (critério diagnóstico KDIGO)</li>
  <li>33% das IRAs são <strong>não oligúricas</strong> (cirurgias, trauma, nefrotoxinas, rabdomiólise)</li>
</ul>

<h4>Sedimentoscopia (Microscopia Urinária)</h4>
<div class="tbl-wrap">
  <table>
    <thead><tr><th>Achado</th><th>Sugere</th></tr></thead>
    <tbody>
      <tr><td>Poucos cilindros e células epiteliais</td><td>IRA pré-renal / funcional — alta chance de reversão</td></tr>
      <tr><td>Cilindros granulosos acastanhados + células epiteliais ↑↑</td><td><strong>Necrose Tubular Aguda (NTA)</strong> — 75% dos casos</td></tr>
      <tr><td>Hematúria + dismorfismo eritrocitário</td><td>Glomerulonefrite / lesão estrutural renal</td></tr>
      <tr><td>Cilindros hemáticos</td><td>Doença glomerular ou vascular</td></tr>
      <tr><td>PMN isolados / aglomerados</td><td>Pielonefrite / necrose papilar</td></tr>
      <tr><td>Leucocitúria + eosinófilos</td><td>Nefrite intersticial aguda</td></tr>
    </tbody>
  </table>
</div>

<h3>Imagem — USG Renal</h3>
<p>Indicada para afastar <strong>IRA pós-renal</strong> (obstrução) e avaliar tamanho renal.</p>

<h3>Novos Biomarcadores de Dano Renal</h3>
<div class="grid">
  <div class="card"><strong>NGAL (urina)</strong><span>Biomarcador de dano tubular — detecta IRA precocemente</span></div>
  <div class="card teal"><strong>[TIMP-2]×[IGFBP7] (urina)</strong><span>Estresse tubular — risco de IRA moderada/grave. Útil nas 1ªs 12h de UTI, pós-cirurgia ou sepse</span></div>
  <div class="card gold"><strong>KIM-1 / IL-18 (urina)</strong><span>Marcadores de risco aumentado (fase pré-AKI)</span></div>
  <div class="card navy"><strong>Cistatina C (soro)</strong><span>Risco de AKI e fase de injúria renal inicial</span></div>
</div>

<h3>Teste de Estresse da Furosemida (FST)</h3>
<div class="alert teal">💊 KDIGO 2026 recomenda (2C adultos / 2B crianças) o FST para avaliar risco de progressão para AKI estágio 3. <br><strong>Atenção:</strong> só realizar em pacientes <mark>normovolêmicos ou hipervolêmicos</mark> — NUNCA em pacientes desidratados!</div>
```

  </div>
</section>

<!-- 6 CAUSAS -->

<section id="s6">
  <div class="sec-header" onclick="toggle(this)">
    <span class="sec-number">06</span>
    <span class="sec-title">Causas de IRA — Pré-renal, Renal, Pós-renal</span>
    <span class="sec-arrow">▼</span>
  </div>
  <div class="sec-body">

```
<div class="grid">
  <div class="card gold">
    <strong>Pré-renal (30–60%)</strong>
    <span>Hipotensão, hipovolemia (diarreia, vômitos, hemorragia), baixo débito cardíaco, sepse, uso de AINEs + IECA/BRA</span>
  </div>
  <div class="card">
    <strong>Renal Intrínseca (20–40%)</strong>
    <span>NTA (isquemia ou nefrotoxinas), glomerulonefrites, vasculites, nefrite intersticial, rabdomiólise</span>
  </div>
  <div class="card navy">
    <strong>Pós-renal (1–10%)</strong>
    <span>HPB, neoplasias, cálculos, fibrose retroperitoneal — diagnosticada por USG renal</span>
  </div>
</div>

<h3>Principais causas de NTA (IRA intrínseca mais comum)</h3>
<ul>
  <li><strong>Isquêmica:</strong> hipotensão, choque (a principal causa)</li>
  <li><strong>Nefrotóxica:</strong> aminoglicosídeos, vancomicina, anfotericina B, contraste iodado, metais pesados</li>
  <li><strong>Por pigmentos:</strong> rabdomiólise (mioglobina), hemólise (hemoglobina)</li>
</ul>

<div class="alert red">🚨 <strong>Anfotericina B</strong> é nefrotóxica! Pode elevar Cr de 1,3 → 3,7. Aciclovir e sulfonamidas também são nefrotóxicos.</div>

<h3>Fatores de Risco para IRA em UTI</h3>
<h4>Não modificáveis</h4>
<p>
  <span class="pill">Idade avançada</span>
  <span class="pill">Sexo masculino</span>
  <span class="pill">Raça negra</span>
  <span class="pill">DRC prévia</span>
  <span class="pill">Proteinúria</span>
  <span class="pill">HAS</span>
  <span class="pill">DM</span>
  <span class="pill">ICC</span>
  <span class="pill">DAC / IAM recente</span>
  <span class="pill">DPOC</span>
  <span class="pill">Doença hepática crônica</span>
</p>
<h4>Potencialmente modificáveis</h4>
<p>
  <span class="pill teal">Sepse</span>
  <span class="pill teal">Trauma</span>
  <span class="pill teal">Cirurgia cardíaca</span>
  <span class="pill teal">Contraste radiológico</span>
  <span class="pill teal">Sobrecarga hídrica</span>
  <span class="pill teal">Drogas nefrotóxicas</span>
  <span class="pill teal">Coloides sintéticos / soluções ricas em cloro</span>
</p>

<h3>Efeitos da IRA em Outros Órgãos (Crosstalk)</h3>
<ul>
  <li><strong>Cérebro:</strong> ↑ KC & G-CSF, permeabilidade vascular, encefalopatia</li>
  <li><strong>Pulmão:</strong> edema, ↑ permeabilidade, susceptibilidade a VAP</li>
  <li><strong>Coração:</strong> ↑ TNF-α, IL-1, apoptose, ↓ função sistólica</li>
  <li><strong>Fígado:</strong> ↑ leucócitos, ↓ antioxidantes, alteração de enzimas</li>
  <li><strong>Intestino:</strong> edema, má absorção, ↑ excreção de K⁺</li>
  <li><strong>Medula óssea:</strong> anemia, coagulopatia, disfunção imune</li>
</ul>
<div class="alert navy">📌 Infecções geram maior mortalidade em pacientes com IRA — a imunossupressão da uremia é real!</div>
```

  </div>
</section>

<!-- 7 FISIOPATOLOGIA -->

<section id="s7">
  <div class="sec-header" onclick="toggle(this)">
    <span class="sec-number">07</span>
    <span class="sec-title">Fisiopatologia</span>
    <span class="sec-arrow">▼</span>
  </div>
  <div class="sec-body">

```
<h3>Autoregulação Glomerular</h3>
<p>A TFG se mantém estável com PAM entre 80–120 mmHg. Abaixo de 80 mmHg → falha da autorregulação → queda da TFG.</p>
<ul>
  <li><strong>Arteriola aferente:</strong> prostaglandinas → vasodilatação (sensível a AINEs)</li>
  <li><strong>Arteriola eferente:</strong> angiotensina II → vasoconstricção (sensível a IECA/BRA)</li>
</ul>
<div class="alert red">⚠️ <strong>AINEs</strong> bloqueiam prostaglandinas vasodilatadoras → ↓ fluxo aferente → ↓ TFG. <strong>IECA/BRA</strong> bloqueiam constrição eferente → ↓ pressão de filtração → ↓ TFG. <em>Ambos são perigosos na IRA!</em></div>

<h3>Por que a medula renal é tão vulnerável à isquemia?</h3>
<ul>
  <li>Recebe apenas <strong>~10% do fluxo plasmático renal</strong></li>
  <li>PO₂ tecidual cai para <strong>10–20 mmHg</strong> (VR sistêmico: ~80 mmHg)</li>
  <li>O ramo ascendente espesso da Alça de Henle consome 50% do O₂ local para transporte ativo de NaCl</li>
  <li>A configuração em "hairpin" gera efeito multiplicador de baixa PO₂</li>
</ul>

<h3>Necrose Tubular Aguda (NTA) — Mecanismo</h3>
<div class="flow">
  <div class="flow-step">Isquemia / nefrotoxina</div>
  <span class="flow-arrow">→</span>
  <div class="flow-step">↓ ATP + ↓ O₂</div>
  <span class="flow-arrow">→</span>
  <div class="flow-step">Lesão celular tubular</div>
  <span class="flow-arrow">→</span>
  <div class="flow-step">Inflamação + lesão microvascular</div>
  <span class="flow-arrow">→</span>
  <div class="flow-step">↓ TFG</div>
</div>
<ul>
  <li>Perda de microvilosidades, desorganização do citoesqueleto</li>
  <li>Células epiteliais descamam → <strong>cilindros que obstruem os túbulos distais</strong></li>
  <li>Backleak de filtrado pelo túbulo proximal</li>
  <li>Citocinas pró-inflamatórias + infiltração de leucócitos</li>
</ul>

<h3>IRA na Sepse</h3>
<p>Em geral <strong>sem hipotensão significativa</strong>. Três mecanismos principais:</p>
<ul>
  <li><strong>Disfunção microvascular:</strong> shunt de fluxo glomerular, perda de glicocalix, estase em capilares peritubulares</li>
  <li><strong>Inflamação:</strong> PAMPs/DAMPs ativam leucócitos → lesão celular</li>
  <li><strong>Reprogramação metabólica:</strong> mitocôndrias lesadas → ↓ produção de ATP</li>
</ul>
```

  </div>
</section>

<!-- 8 EVOLUÇÃO CLÍNICA -->

<section id="s8">
  <div class="sec-header" onclick="toggle(this)">
    <span class="sec-number">08</span>
    <span class="sec-title">Evolução Clínica e Trajetórias</span>
    <span class="sec-arrow">▼</span>
  </div>
  <div class="sec-body">

```
<h3>Fases da IRA</h3>
<div class="tbl-wrap">
  <table>
    <thead><tr><th>Fase</th><th>Características</th><th>Conduta</th></tr></thead>
    <tbody>
      <tr><td><strong>Inicial</strong></td><td>Pode ser súbito (ex.: acidente ofídico) ou insidioso (ATB)</td><td>Identificar e tratar a causa</td></tr>
      <tr><td><strong>Oligúrica</strong></td><td>DU ↓↓ — quadros mais graves, maior mortalidade. Pode estar ausente (33%)</td><td>Restrição hídrica cautelosa + furosemida</td></tr>
      <tr><td><strong>Poliúrica</strong></td><td>DU 2–5 L/dia — defeitos tubulares na concentração. Risco de desidratação e distúrbios eletrolíticos</td><td><strong>Estimular ingestão hídrica!</strong></td></tr>
      <tr><td><strong>Recuperação (NTA)</strong></td><td>Queda espontânea das escórias. <mark>7 a 21 dias</mark> para recuperação</td><td>Manter suporte</td></tr>
    </tbody>
  </table>
</div>

<div class="alert gold">⚠️ IRA oligúrica é <strong>grave</strong> — pode evoluir para óbito! IRA não-oligúrica tem melhor prognóstico.</div>

<h3>Trajetórias: AKI → AKD → DRC</h3>
<ul>
  <li><strong>AKI estágio 1</strong> resolvido → sem AKD → sem DRC (melhor cenário)</li>
  <li><strong>AKI estágio 2</strong> → risco de AKD + progressão para DRC</li>
  <li><strong>AKI estágio 3</strong> → AKD + possível falência renal permanente</li>
</ul>
<div class="alert teal">📌 Sobreviventes de IRA têm maior chance de desenvolver <strong>Doença Renal Crônica</strong> — acompanhamento obrigatório!</div>
```

  </div>
</section>

<!-- 9 TRATAMENTO -->

<section id="s9">
  <div class="sec-header" onclick="toggle(this)">
    <span class="sec-number">09</span>
    <span class="sec-title">Prevenção e Tratamento</span>
    <span class="sec-arrow">▼</span>
  </div>
  <div class="sec-body">

```
<h3>Medidas Gerais por Estágio (KDIGO)</h3>
<div class="tbl-wrap">
  <table>
    <thead><tr><th>Medida</th><th>Alto risco</th><th>Est. 1</th><th>Est. 2</th><th>Est. 3</th></tr></thead>
    <tbody>
      <tr><td>Suspender nefrotóxicos</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td></tr>
      <tr><td>Garantir volemia e pressão de perfusão</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td></tr>
      <tr><td>Monitorar Cr e DU</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td></tr>
      <tr><td>Evitar hiperglicemia</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td></tr>
      <tr><td>Considerar alternativas ao contraste</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td></tr>
      <tr><td>Ajuste de doses de drogas</td><td>—</td><td>—</td><td>✅</td><td>✅</td></tr>
      <tr><td>Considerar TRS / UTI</td><td>—</td><td>—</td><td>✅</td><td>✅</td></tr>
      <tr><td>Evitar cateter em subclávia</td><td>—</td><td>—</td><td>—</td><td>✅ (preferir jugular D)</td></tr>
    </tbody>
  </table>
</div>

<h3>Reposição Volêmica</h3>
<div class="alert teal">💧 Repor volume é essencial na IRA pré-renal — mas <strong>sobrecarga hídrica também é prejudicial</strong>! Causa edema cerebral, pulmonar, renal e piora da função.</div>

<h4>Fluidos: benefício × risco (evidências)</h4>
<ul>
  <li>🟢 <strong>Cristaloides balanceados</strong> (Ringer Lactato): melhor opção</li>
  <li>🟡 <strong>SF 0,9%</strong>: aceitável, mas rico em cloro → pode piorar função renal</li>
  <li>🟡 <strong>Albumina</strong>: papel em casos específicos (cirrose, sepse)</li>
  <li>🔴 <strong>HES (amido)</strong>: contraindicado — causa NTA!</li>
  <li>🔴 <strong>Gelatinas</strong>: baixa evidência de benefício</li>
</ul>

<h3>Vasopressores e Hemodinâmica</h3>
<ul>
  <li>Meta de PAM: <strong>≥ 65 mmHg</strong> (no choque séptico)</li>
  <li>Vasopressor de escolha: <strong>Norepinefrina</strong></li>
  <li>Vasopressina: segunda linha</li>
  <li>Dopamina em baixa dose NÃO protege os rins (evidência obsoleta)</li>
</ul>

<h3>Manejo de Eletrólitos</h3>
<h4>Hipercalemia — alterações no ECG</h4>
<ul>
  <li>K⁺ ↑ → Onda P achatada → QRS alargado → Onda T apiculada (em tenda)</li>
  <li>K⁺ &gt; 6,5: indicação de diálise urgente</li>
</ul>
<h4>Acidose Metabólica</h4>
<ul>
  <li>Bicarbonato IV: considerar se pH &lt; 7,2 com acidose metabólica pura</li>
  <li><strong>Contraindicações do Bicarbonato:</strong> acidose respiratória, alcalose metabólica, DPOC descompensado, hipocalemia</li>
</ul>
```

  </div>
</section>

<!-- 10 DIÁLISE -->

<section id="s10">
  <div class="sec-header" onclick="toggle(this)">
    <span class="sec-number">10</span>
    <span class="sec-title">Terapia Renal Substitutiva (TRS / Diálise)</span>
    <span class="sec-arrow">▼</span>
  </div>
  <div class="sec-body">

```
<h3>Indicações URGENTES — Mnemônico AEIOU</h3>
<div class="mnemonic">
  <div><span class="letra">A</span> <strong>Acidose</strong> metabólica severa (pH &lt; 7,1) refratária ao tratamento clínico</div>
  <div><span class="letra">E</span> <strong>Eletrólitos</strong> — hipercalemia grave (K⁺ &gt; 6,5 ou com alteração de ECG)</div>
  <div><span class="letra">I</span> <strong>Intoxicações</strong> por certos alcoóis ou drogas dialisáveis</div>
  <div><span class="letra">O</span> <strong>Overload</strong> (sobrecarga hídrica) refratária a diuréticos</div>
  <div><span class="letra">U</span> <strong>Uremia</strong> — encefalopatia, pericardite, náuseas, vômitos, soluços, flapping, abalos musculares</div>
</div>

<h3>Início Precoce vs Tardio — STARRT-AKI (NEJM 2020)</h3>
<ul>
  <li>3.019 pacientes graves em UTI, 168 hospitais, 15 países</li>
  <li>TRS precoce (12h) vs tardio (indicação clínica presente)</li>
  <li><strong>Resultado:</strong> sem diferença de mortalidade em 90 dias (44% em ambos os grupos)</li>
  <li>TRS precoce: mais dependência de diálise entre sobreviventes</li>
</ul>
<div class="alert red">🚨 Início precoce de TRS na IRA geralmente <strong>não é benéfico</strong> — pode ser prejudicial, atrasar recuperação e aumentar uso de recursos de saúde. Aguardar indicação clínica!</div>

<h3>Modalidades Dialíticas</h3>
<h4>Intermitentes</h4>
<p><span class="pill navy">DPI</span> <span class="pill navy">HD (Hemodiálise)</span> <span class="pill navy">UF (Ultrafiltração)</span></p>
<h4>Contínuas (CRRT)</h4>
<p><span class="pill teal">SCUF</span> <span class="pill teal">CVVH</span> <span class="pill teal">CVVHD</span> <span class="pill teal">CVVHDF</span> <span class="pill teal">DPC</span> <span class="pill teal">Plasmafiltração</span></p>
<h4>Híbridas</h4>
<p><span class="pill gold" style="color:#333">SLED</span> <span class="pill gold" style="color:#333">SLEDf</span></p>

<h3>Fatores que influenciam a indicação de TRS</h3>
<div class="grid">
  <div class="card"><strong>Gravidade da IRA</strong><span>Creatinina, DU, eletrólitos, ácido-base, uremia</span></div>
  <div class="card teal"><strong>Gravidade da doença crítica</strong><span>Evento causador, disfunção de outros órgãos, sobrecarga hídrica</span></div>
  <div class="card gold"><strong>Riscos do procedimento</strong><span>Hipotensão, anticoagulação, perda de nutrientes e drogas</span></div>
  <div class="card navy"><strong>Outros fatores</strong><span>Disponibilidade de máquinas/equipe, prognóstico, custo</span></div>
</div>

<h3>Performance Status de Karnofski</h3>
<p>Usado para avaliar a condição funcional basal do paciente e guiar decisões de TRS (especialmente em idosos com baixo status funcional):</p>
<ul>
  <li>100–80: ativo, com poucos sintomas</li>
  <li>70–50: necessita assistência parcial</li>
  <li>40–20: acamado, depende de cuidados</li>
  <li>10: moribundo</li>
</ul>
<div class="alert gold">📋 Um paciente acamado desde AVE há 3 anos com KPS 20–30 — a decisão de diálise deve considerar o <strong>prognóstico global</strong>, futilidade e qualidade de vida.</div>
```

  </div>
</section>

<!-- QUESTÃO DE PROVA -->

<section>
  <div class="sec-header" onclick="toggle(this)">
    <span class="sec-number">🎓</span>
    <span class="sec-title">Questão de Residência (UNICAMP 2022)</span>
    <span class="sec-arrow">▼</span>
  </div>
  <div class="sec-body">
    <div class="alert navy">Homem, 72 anos, ↓ diurese 2 dias após cateterismo cardíaco. Usou anti-inflamatório 1 semana antes. Cr basal 1,2 → atual 3,2. Assimetria de pulsos distais, livedo reticular. Urina: 15 leuco/campo, 10 hemácias/campo, cilindros hialinos e granulosos. Eosinófilos 730/mm³.</div>
    <h3>Análise:</h3>
    <ul>
      <li>Cateterismo → potencial embolização de colesterol para vasos renais</li>
      <li>Livedo reticular + assimetria de pulsos = sinais sistêmicos de ateroembolismo</li>
      <li>Eosinofilia periférica é característica da doença ateroembólica</li>
      <li>Nefrite intersticial poderia ter eosinófilos, mas o quadro sistêmico aponta para ateroembolia</li>
    </ul>
    <div class="alert teal">✅ <strong>Resposta: (A) Doença Ateroembólica</strong></div>
  </div>
</section>

</main>

<footer>
  Guia de estudo elaborado por Daniel Guimarães — FAMETRO 7º Período · Nefrologia<br>
  Referências: KDIGO 2012 & 2026 Draft · STARRT-AKI (NEJM 2020) · Bywaters (BMJ 1990) · Chertow et al. (JASN 2005)
</footer>

<script>
function toggle(header) {
  header.classList.toggle('open');
  const body = header.nextElementSibling;
  body.classList.toggle('open');
}
// Open first section by default — already done in HTML
</script>

</body>
</html>
