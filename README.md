
<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Fala Real — Alemão (e inglês) de verdade, não de sala de aula</title>
<meta name="description" content="Pratique alemão e inglês de verdade — sotaque, ruído de fundo e interrupções, pra quem quer se envolver de verdade na vida daqui. Não o idioma de sala de aula.">

<!-- Open Graph / WhatsApp / Facebook -->
<meta property="og:type" content="website">
<meta property="og:title" content="Fala Real — Alemão e inglês de verdade">
<meta property="og:description" content="Sotaque, ruído de fundo, interrupções — pratique o idioma como ele realmente acontece no dia a dia, pra quem quer se envolver de verdade.">
<meta property="og:image" content="/og-image.png">
<meta property="og:image:width" content="1200">
<meta property="og:image:height" content="630">
<meta property="og:url" content="https://falareal-site-17.vercel.app">
<link rel="canonical" href="https://falareal-site-17.vercel.app">

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "SoftwareApplication",
  "name": "Fala Real",
  "applicationCategory": "EducationalApplication",
  "operatingSystem": "Web",
  "description": "Pratique alemão e inglês de verdade — sotaque, ruído de fundo e interrupções, como realmente acontece no dia a dia.",
  "url": "https://falareal-site-17.vercel.app",
  "inLanguage": ["pt-BR", "de", "en"],
  "offers": {
    "@type": "Offer",
    "availability": "https://schema.org/PreOrder"
  }
}
</script>

<!-- Twitter -->
<meta name="twitter:card" content="summary_large_image">
<meta name="twitter:title" content="Fala Real — Alemão e inglês de verdade">
<meta name="twitter:description" content="Sotaque, ruído de fundo, interrupções — pratique o idioma como ele realmente acontece no dia a dia, pra quem quer se envolver de verdade.">
<meta name="twitter:image" content="/og-image.png">

<link rel="icon" type="image/png" href="/favicon-32.png">
<link rel="apple-touch-icon" href="/favicon.png">
<meta name="theme-color" content="#12181f">

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Fraunces:opsz,wght@9..144,400;9..144,500;9..144,600;9..144,700&family=IBM+Plex+Sans:wght@400;500;600&family=IBM+Plex+Mono:wght@400;500&display=swap" rel="stylesheet">

<!-- Vercel Web Analytics — mostra quantos visitantes reais o site recebe -->
<script>
  window.va = window.va || function () { (window.vaq = window.vaq || []).push(arguments); };
</script>
<script defer src="/_vercel/insights/script.js"></script>

<style>
  :root{
    --ink:#12181f;
    --ink-soft:#1c2530;
    --paper:#f4efe6;
    --amber:#f0a63a;
    --teal:#3e6b63;
    --rust:#c1483d;
    --line: rgba(244,239,230,0.14);
    --display: 'Fraunces', serif;
    --body: 'IBM Plex Sans', sans-serif;
    --mono: 'IBM Plex Mono', monospace;
  }
  *{margin:0;padding:0;box-sizing:border-box;}
  html{scroll-behavior:smooth;}
  body{
    background:var(--ink);
    color:var(--paper);
    font-family:var(--body);
    line-height:1.5;
    -webkit-font-smoothing:antialiased;
    overflow-x:hidden;
  }
  a{color:inherit;text-decoration:none;}
  img,svg{display:block;max-width:100%;}
  ::selection{background:var(--amber);color:var(--ink);}
  :focus-visible{outline:2px solid var(--amber); outline-offset:3px;}

  .wrap{max-width:1080px;margin:0 auto;padding:0 24px;}

  /* NAV */
  nav{
    position:sticky;top:0;z-index:50;
    background:rgba(18,24,31,0.85);
    backdrop-filter: blur(8px);
    border-bottom:1px solid var(--line);
  }
  nav .wrap{display:flex;align-items:center;justify-content:space-between;height:68px;}
  .logo{font-family:var(--display);font-weight:600;font-size:1.25rem;letter-spacing:-0.02em;}
  .logo span{color:var(--amber);}
  .nav-cta{
    font-family:var(--mono);font-size:0.8rem;letter-spacing:0.02em;
    background:var(--amber); color:var(--ink); padding:9px 18px; border-radius:100px;
    transition: transform .15s ease;
  }
  .nav-cta:hover{transform:translateY(-1px);}

  /* LANG TOGGLE */
  .lang-toggle{
    display:flex; gap:4px; background:var(--ink-soft); border:1px solid var(--line);
    padding:4px; border-radius:100px;
  }
  .lang-toggle button{
    font-family:var(--mono); font-size:0.76rem; letter-spacing:0.02em;
    background:transparent; border:none; color:rgba(244,239,230,0.5);
    padding:7px 14px; border-radius:100px; cursor:pointer;
    transition: background .15s ease, color .15s ease;
  }
  .lang-toggle button.active{background:var(--amber); color:var(--ink);}
  .nav-right{display:flex; align-items:center; gap:14px;}

  /* language visibility: German is the flagship, shown by default */
  body.lang-en .lang-de{display:none;}
  body.lang-de .lang-en{display:none;}

  /* HERO */
  header.hero{
    padding:96px 0 64px;
    position:relative;
  }
  .hero-top{
    display:grid; grid-template-columns:1.15fr 0.85fr; gap:48px; align-items:center;
  }
  @media (max-width:900px){
    .hero-top{grid-template-columns:1fr; gap:8px;}
    .hero-visual{order:-1; max-width:280px; margin:0 auto 8px;}
  }
  .hero-visual{width:100%;}
  .hero-illustration-svg{width:100%; height:auto; display:block;}
  .hero-illustration-svg .bubble{transition: transform .3s ease;}
  .hero-illustration-svg .bubble-loud{animation: bubble-pulse 2.6s ease-in-out infinite;}
  @keyframes bubble-pulse{
    0%, 100%{ transform: scale(1); }
    50%{ transform: scale(1.03); }
  }
  .hero-illustration-svg .burst{animation: burst-flicker 1.8s ease-in-out infinite;}
  @keyframes burst-flicker{
    0%, 100%{ opacity:0.5; }
    50%{ opacity:1; }
  }
  @media (prefers-reduced-motion: reduce){
    .hero-illustration-svg .bubble-loud, .hero-illustration-svg .burst{animation:none;}
  }
  .eyebrow{
    font-family:var(--mono); font-size:0.78rem; letter-spacing:0.12em; text-transform:uppercase;
    color:var(--teal); background:rgba(62,107,99,0.18); border:1px solid rgba(62,107,99,0.4);
    display:inline-block; padding:6px 14px; border-radius:100px; margin-bottom:28px;
  }
  h1{
    font-family:var(--display);
    font-weight:600;
    font-size:clamp(2.4rem, 6vw, 4.4rem);
    line-height:1.02;
    letter-spacing:-0.02em;
    max-width:16ch;
  }
  h1 em{font-style:italic; color:var(--amber); font-weight:500;}
  .sub{
    margin-top:28px;
    font-size:clamp(1.05rem, 2vw, 1.3rem);
    color:rgba(244,239,230,0.72);
    max-width:46ch;
  }
  .hero-actions{margin-top:40px;display:flex;gap:16px;flex-wrap:wrap;align-items:center;}
  .btn-primary{
    font-family:var(--body); font-weight:600; font-size:1rem;
    background:var(--amber); color:var(--ink); padding:16px 30px; border-radius:100px;
    border:none; cursor:pointer;
    transition: transform .15s ease, box-shadow .15s ease;
    box-shadow: 0 0 0 rgba(240,166,58,0);
  }
  .btn-primary:hover{transform:translateY(-2px); box-shadow:0 8px 24px rgba(240,166,58,0.25);}
  .btn-ghost{
    font-family:var(--mono); font-size:0.85rem; color:rgba(244,239,230,0.6);
    border-bottom:1px solid rgba(244,239,230,0.3); padding-bottom:2px;
  }

  /* WAVEFORM SIGNATURE */
  .wave-stage{
    margin-top:72px;
    border:1px solid var(--line);
    border-radius:20px;
    background:linear-gradient(180deg, var(--ink-soft), var(--ink));
    padding:32px 28px 24px;
    overflow:hidden;
  }
  .wave-labels{
    display:flex; justify-content:space-between; font-family:var(--mono);
    font-size:0.72rem; color:rgba(244,239,230,0.45); letter-spacing:0.04em;
    margin-bottom:14px; text-transform:uppercase;
  }
  .wave-labels .active{color:var(--amber);}
  svg#wave{width:100%; height:110px;}
  .wave-caption{
    margin-top:12px; font-family:var(--mono); font-size:0.78rem; color:rgba(244,239,230,0.5);
  }

  /* SECTION SHARED */
  section{padding:96px 0;}
  .section-head{max-width:56ch; margin-bottom:56px;}
  .kicker{
    font-family:var(--mono); font-size:0.78rem; letter-spacing:0.1em; text-transform:uppercase;
    color:var(--amber); margin-bottom:14px; display:block;
  }
  h2{
    font-family:var(--display); font-weight:600; font-size:clamp(1.8rem,3.6vw,2.6rem);
    letter-spacing:-0.01em; line-height:1.1;
  }
  .lede{margin-top:16px; color:rgba(244,239,230,0.68); font-size:1.05rem; max-width:52ch;}

  /* COMPARISON */
  .compare{
    display:grid; grid-template-columns:1fr 1fr; gap:1px;
    background:var(--line); border:1px solid var(--line); border-radius:16px; overflow:hidden;
  }
  .compare > div{background:var(--ink); padding:32px;}
  .compare h3{font-family:var(--mono); font-size:0.85rem; text-transform:uppercase; letter-spacing:0.06em; margin-bottom:18px;}
  .compare .lab h3{color:rgba(244,239,230,0.45);}
  .compare .real h3{color:var(--amber);}
  .compare ul{list-style:none;}
  .compare li{
    padding:10px 0; border-top:1px solid var(--line); font-size:0.98rem;
    color:rgba(244,239,230,0.8);
    transition: padding-left .2s ease, color .2s ease;
  }
  .compare li:first-child{border-top:none;}
  .compare .real li{color:var(--paper);}
  .compare li:hover{padding-left:8px;}
  .compare .real li:hover{color:var(--amber);}
  .compare .lab li:hover{color:rgba(244,239,230,0.95);}

  @media (max-width:720px){
    .compare{grid-template-columns:1fr;}
  }

  /* LEVELS TIMELINE */
  .levels{position:relative;}
  .level-row{
    display:grid; grid-template-columns:88px 1fr; gap:24px;
    padding:28px 0; border-top:1px solid var(--line);
    position:relative;
    transition: background .25s ease;
  }
  .level-row:hover{background:rgba(244,239,230,0.02);}
  .level-row:last-child{border-bottom:1px solid var(--line);}
  .level-num{
    font-family:var(--mono); font-size:0.85rem; color:rgba(244,239,230,0.4);
    padding-top:4px;
    transition: transform .25s ease, color .25s ease;
  }
  .level-row:hover .level-num{transform:translateX(4px); color:var(--amber);}
  .level-row[data-level="4"]:hover .level-num{color:var(--rust);}
  .level-row[data-level="4"] .level-num{color:var(--rust);}
  .level-title{
    font-family:var(--display); font-weight:600; font-size:1.35rem; margin-bottom:8px;
  }
  .level-desc{color:rgba(244,239,230,0.65); font-size:0.98rem; max-width:56ch;}
  .level-tags{margin-top:12px; display:flex; gap:8px; flex-wrap:wrap;}
  .level-tags span{
    font-family:var(--mono); font-size:0.7rem; text-transform:uppercase; letter-spacing:0.04em;
    border:1px solid var(--line); color:rgba(244,239,230,0.55);
    padding:4px 10px; border-radius:100px;
  }

  .level-audio-btn{
    margin-top:16px; display:inline-flex; align-items:center; gap:6px;
    font-family:var(--body); font-weight:600; font-size:0.85rem;
    background:transparent; color:var(--paper); border:1px solid var(--teal);
    padding:9px 16px; border-radius:100px; cursor:pointer;
    transition: background .15s ease;
  }
  .level-audio-btn:hover{background:rgba(62,107,99,0.18);}
  .level-audio-btn:disabled{opacity:0.55; cursor:default;}
  .level-audio-btn.playing{background:var(--teal);}
  .level-row[data-level="4"] .level-audio-btn{border-color:var(--rust);}
  .level-row[data-level="4"] .level-audio-btn.playing{background:var(--rust);}

  /* INTERACTIVE DEMO */
  .demo-grid{
    display:grid; grid-template-columns:1fr 1fr; gap:24px;
  }
  @media (max-width:820px){.demo-grid{grid-template-columns:1fr;}}
  .demo-card{
    border:1px solid var(--line); border-radius:20px; padding:32px;
    background:var(--ink-soft);
    display:flex; flex-direction:column;
    transition: transform .25s ease, border-color .25s ease, box-shadow .25s ease;
  }
  .demo-card:hover{
    transform:translateY(-4px);
    border-color:rgba(240,166,58,0.35);
    box-shadow:0 16px 40px rgba(0,0,0,0.25);
  }
  .demo-card h3{
    font-family:var(--display); font-weight:600; font-size:1.3rem; margin-bottom:8px;
  }
  .demo-sub{color:rgba(244,239,230,0.6); font-size:0.92rem; margin-bottom:24px;}
  .btn-full{width:100%; margin-top:auto;}

  /* level simulator */
  .level-display{display:flex; align-items:baseline; gap:12px; margin-bottom:10px;}
  .level-badge{
    font-family:var(--mono); font-size:1.6rem; font-weight:500; color:var(--amber);
    transition: color .2s ease;
  }
  .level-tier{
    font-family:var(--mono); font-size:0.78rem; text-transform:uppercase; letter-spacing:0.06em;
    color:rgba(244,239,230,0.5);
  }
  .level-tags-live{display:flex; gap:8px; flex-wrap:wrap; min-height:52px; align-items:flex-start;}
  .level-tags-live span{
    font-family:var(--mono); font-size:0.72rem; letter-spacing:0.02em;
    background:rgba(240,166,58,0.12); border:1px solid rgba(240,166,58,0.35); color:var(--paper);
    padding:5px 11px; border-radius:100px;
    animation: tag-in .3s ease both;
  }
  @keyframes tag-in{from{opacity:0; transform:translateY(4px) scale(0.9);} to{opacity:1; transform:none;}}
  .mini-wave-wrap{margin:18px 0 24px; border:1px solid var(--line); border-radius:12px; padding:10px 14px; background:var(--ink);}
  svg#mini-wave{width:100%; height:60px;}

  .audio-row{display:flex; align-items:center; gap:12px; margin-bottom:16px;}
  .btn-audio{
    font-family:var(--body); font-weight:600; font-size:0.9rem;
    background:transparent; color:var(--paper); border:1px solid var(--teal);
    padding:12px 20px; border-radius:100px; cursor:pointer;
    transition: background .15s ease, transform .15s ease;
  }
  .btn-audio:hover{background:rgba(62,107,99,0.18);}
  .btn-audio:disabled{opacity:0.5; cursor:default;}
  .btn-audio.playing{background:var(--teal); border-color:var(--teal);}
  .audio-status{font-family:var(--mono); font-size:0.75rem; color:rgba(244,239,230,0.45);}

  /* streak */
  .streak-hero{display:flex; align-items:center; gap:16px; margin-bottom:20px;}
  .flame{font-size:2.2rem; filter:grayscale(1) opacity(0.4); transition: filter .3s ease, transform .2s ease;}
  .flame.lit{filter:none; transform:scale(1.08);}
  .streak-num{font-family:var(--display); font-weight:600; font-size:2.1rem; line-height:1;}
  .streak-label{font-family:var(--mono); font-size:0.75rem; color:rgba(244,239,230,0.5); text-transform:uppercase; letter-spacing:0.04em;}
  .streak-dots{display:flex; gap:8px; margin-bottom:20px;}
  .streak-dots .dot{
    width:14px; height:14px; border-radius:4px; background:var(--ink); border:1px solid var(--line);
    transition: background .2s ease, border-color .2s ease;
  }
  .streak-dots .dot.filled{background:var(--amber); border-color:var(--amber);}
  .xp-row{display:flex; align-items:center; gap:12px; margin-bottom:22px;}
  .xp-bar-track{flex:1; height:8px; border-radius:100px; background:var(--ink); border:1px solid var(--line); overflow:hidden;}
  .xp-bar-fill{height:100%; width:0%; background:var(--teal); border-radius:100px; transition:width .4s ease;}
  .xp-label{font-family:var(--mono); font-size:0.75rem; color:rgba(244,239,230,0.5); white-space:nowrap;}
  .reward-toast{
    margin-top:14px; font-family:var(--mono); font-size:0.82rem; color:var(--amber);
    min-height:1.2em; opacity:0; transition:opacity .3s ease;
  }
  .reward-toast.show{opacity:1;}

  .btn-share{
    width:100%; margin-top:14px;
    font-family:var(--body); font-weight:600; font-size:0.92rem;
    background:linear-gradient(135deg, var(--amber), var(--rust)); color:var(--ink);
    border:none; padding:13px 20px; border-radius:100px; cursor:pointer;
    transition: transform .15s ease;
  }
  .btn-share:hover{transform:translateY(-1px);}

  .share-preview{margin-top:18px;}
  .share-preview canvas{
    width:100%; max-width:280px; display:block; margin:0 auto 14px;
    border-radius:16px; border:1px solid var(--line);
  }
  .share-actions{display:flex; gap:10px; flex-wrap:wrap; justify-content:center;}

  /* confetti burst */
  .confetti-piece{
    position:fixed; top:0; left:0; width:8px; height:14px; pointer-events:none; z-index:999;
    border-radius:2px; opacity:0.95;
  }
  @keyframes confetti-fall{
    0%{ transform: translate(0,0) rotate(0deg); opacity:1; }
    100%{ transform: translate(var(--drift), 100vh) rotate(var(--spin)); opacity:0; }
  }

  /* QUICK DIAGNOSTIC QUIZ */
  .quiz-card{
    max-width:560px; margin:0 auto; border:1px solid var(--line); border-radius:20px;
    background:var(--ink-soft); padding:40px 36px; text-align:center;
  }
  .quiz-step{display:none;}
  .quiz-step.active{display:block; animation: quiz-fade-in .35s ease;}
  @keyframes quiz-fade-in{ from{opacity:0; transform:translateY(8px);} to{opacity:1; transform:none;} }
  .quiz-question{
    font-family:var(--display); font-weight:600; font-size:1.3rem; margin-bottom:24px;
  }
  .quiz-options{display:flex; flex-direction:column; gap:10px;}
  .quiz-option{
    font-family:var(--body); font-size:0.95rem; color:var(--paper);
    background:var(--ink); border:1px solid var(--line); border-radius:12px;
    padding:14px 18px; text-align:left; cursor:pointer;
    transition: border-color .2s ease, background .2s ease, transform .15s ease;
  }
  .quiz-option:hover{border-color:var(--amber); background:rgba(240,166,58,0.08); transform:translateX(3px);}
  .quiz-result-icon{font-size:2.4rem; margin-bottom:12px;}
  .quiz-result-title{
    font-family:var(--display); font-weight:600; font-size:1.25rem; margin-bottom:12px;
  }
  .quiz-result-title span{color:var(--amber);}
  .quiz-result-desc{color:rgba(244,239,230,0.7); font-size:0.95rem; margin-bottom:24px; max-width:44ch; margin-left:auto; margin-right:auto;}
  .quiz-progress{display:flex; justify-content:center; gap:8px; margin-top:28px;}
  .quiz-dot{width:8px; height:8px; border-radius:50%; background:var(--line); transition: background .3s ease, transform .3s ease;}
  .quiz-dot.active{background:var(--amber); transform:scale(1.3);}
  .quiz-dot.done{background:var(--teal);}
  .quiz-summary{
    font-family:var(--mono); font-size:0.82rem; color:var(--amber);
    background:rgba(240,166,58,0.1); border:1px solid rgba(240,166,58,0.3);
    padding:10px 16px; border-radius:10px; margin:0 0 20px; display:none;
  }
  .quiz-summary.show{display:block;}

  /* PHONE MOCKUP PREVIEW */
  .phone-mockup-wrap{display:flex; justify-content:center;}
  .phone-frame{
    width:100%; max-width:380px;
    background:var(--ink-soft); border:1px solid var(--line); border-radius:36px;
    padding:14px 16px 28px; position:relative;
    box-shadow:0 30px 70px rgba(0,0,0,0.35);
  }
  .phone-notch{
    width:100px; height:18px; background:var(--ink); border-radius:0 0 14px 14px;
    margin:0 auto 14px;
  }
  .phone-topbar{
    display:flex; justify-content:space-between; align-items:center;
    margin-bottom:16px; padding:0 4px;
  }
  .phone-level-badge{
    font-family:var(--mono); font-size:0.72rem; color:var(--amber);
    background:rgba(240,166,58,0.12); border:1px solid rgba(240,166,58,0.35);
    padding:5px 12px; border-radius:100px;
  }
  .phone-mic-status{
    font-family:var(--mono); font-size:0.7rem; color:rgba(244,239,230,0.5);
    display:flex; align-items:center; gap:6px;
  }
  .phone-mic-status .dot{
    width:7px; height:7px; border-radius:50%; background:var(--rust);
    animation: dot-blink 1.4s ease-in-out infinite;
  }
  @keyframes dot-blink{ 0%,100%{opacity:1;} 50%{opacity:0.3;} }

  .phone-chat{display:flex; flex-direction:column; gap:12px; min-height:220px;}
  .chat-bubble{
    max-width:82%; padding:12px 16px; border-radius:16px; font-size:0.92rem; line-height:1.4;
  }
  .chat-bubble.ai{
    background:var(--ink); border:1px solid var(--line); color:var(--paper);
    align-self:flex-start; border-bottom-left-radius:4px;
  }
  .chat-bubble.user{
    background:var(--teal); color:var(--paper);
    align-self:flex-end; border-bottom-right-radius:4px;
  }
  .chat-bubble.feedback{
    align-self:center; max-width:100%;
    background:rgba(240,166,58,0.1); border:1px dashed rgba(240,166,58,0.4);
    color:rgba(244,239,230,0.85); font-size:0.85rem; border-radius:12px;
  }

  .phone-mic-btn{
    width:56px; height:56px; border-radius:50%; margin:22px auto 0;
    background:var(--amber); display:flex; align-items:center; justify-content:center;
    font-size:1.3rem; position:relative;
  }
  .mic-pulse{
    position:absolute; inset:0; border-radius:50%; border:2px solid var(--amber);
    animation: mic-pulse-anim 2s ease-out infinite;
  }
  .mic-pulse-2{ animation-delay:1s; }
  @keyframes mic-pulse-anim{
    0%{ transform:scale(1); opacity:0.7; }
    100%{ transform:scale(1.8); opacity:0; }
  }
  @media (prefers-reduced-motion: reduce){
    .mic-pulse{animation:none; display:none;}
    .phone-mic-status .dot{animation:none;}
  }

  /* HOW IT WORKS */
  .steps{display:grid; grid-template-columns:repeat(3,1fr); gap:28px;}
  .step{
    border:1px solid var(--line); border-radius:16px; padding:28px;
    transition: transform .25s ease, border-color .25s ease;
  }
  .step:hover{transform:translateY(-3px); border-color:rgba(62,107,99,0.5);}
  .step .n{font-family:var(--mono); color:var(--teal); font-size:0.85rem; margin-bottom:14px; display:block;}
  .step h4{font-family:var(--display); font-weight:600; font-size:1.15rem; margin-bottom:10px;}
  .step p{color:rgba(244,239,230,0.65); font-size:0.95rem;}
  @media (max-width:820px){.steps{grid-template-columns:1fr;}}

  /* FINAL CTA */
  .cta-band{
    background:var(--ink-soft); border-top:1px solid var(--line); border-bottom:1px solid var(--line);
  }
  .cta-inner{text-align:left; max-width:640px;}
  .cta-inner h2{margin-bottom:16px;}
  .email-form{
    margin-top:32px; display:flex; gap:12px; flex-wrap:wrap;
  }
  .email-form input[type=email]{
    flex:1; min-width:220px;
    background:var(--ink); border:1px solid var(--line); color:var(--paper);
    padding:15px 18px; border-radius:100px; font-family:var(--body); font-size:0.95rem;
  }
  .email-form input[type=email]::placeholder{color:rgba(244,239,230,0.4);}
  .form-note{margin-top:14px; font-family:var(--mono); font-size:0.78rem; color:rgba(244,239,230,0.4);}
  .thanks{
    display:none; margin-top:20px; padding:16px 20px; border:1px solid var(--teal);
    background:rgba(62,107,99,0.15); border-radius:12px; font-size:0.95rem;
  }
  .thanks p{margin:0;}

  .referral-box{margin-top:18px; padding-top:16px; border-top:1px dashed rgba(244,239,230,0.2);}
  .referral-title{font-family:var(--display); font-weight:600; font-size:1.05rem; margin-bottom:6px;}
  .referral-desc{color:rgba(244,239,230,0.65); font-size:0.88rem; margin-bottom:14px;}
  .referral-link-row{display:flex; gap:8px; margin-bottom:12px;}
  .referral-input{
    flex:1; min-width:0; background:var(--ink); border:1px solid var(--line); color:rgba(244,239,230,0.8);
    padding:10px 14px; border-radius:10px; font-family:var(--mono); font-size:0.78rem;
  }

  footer{padding:40px 0; border-top:1px solid var(--line);}
  footer .wrap{display:flex; justify-content:space-between; align-items:center; flex-wrap:wrap; gap:12px;}
  footer p{font-family:var(--mono); font-size:0.78rem; color:rgba(244,239,230,0.4);}
  .version-tag{font-family:var(--mono); font-size:0.68rem; color:rgba(244,239,230,0.3); font-weight:400; letter-spacing:0.02em;}

  [data-reveal]{opacity:0; transform:translateY(16px); transition:opacity .6s ease, transform .6s ease;}
  [data-reveal].in{opacity:1; transform:translateY(0);}

  /* cascata: itens dentro de cada seção revelada aparecem em sequência, não todos de uma vez */
  .steps .step, .demo-grid .demo-card, .compare > div, .levels .level-row{
    opacity:0; transform:translateY(14px);
    transition: opacity .5s ease, transform .5s ease;
  }
  .steps.in .step, .demo-grid.in .demo-card, .compare.in > div, .levels.in .level-row{
    opacity:1; transform:translateY(0);
  }
  .steps .step:nth-child(1), .demo-grid .demo-card:nth-child(1), .compare > div:nth-child(1), .levels .level-row:nth-child(1){transition-delay:0s;}
  .steps .step:nth-child(2), .demo-grid .demo-card:nth-child(2), .compare > div:nth-child(2), .levels .level-row:nth-child(2){transition-delay:.1s;}
  .steps .step:nth-child(3), .levels .level-row:nth-child(3){transition-delay:.2s;}
  .levels .level-row:nth-child(4){transition-delay:.3s;}

  @media (prefers-reduced-motion: reduce){
    [data-reveal]{opacity:1; transform:none; transition:none;}
    html{scroll-behavior:auto;}
  }
</style>
</head>
<body class="lang-de">

<nav>
  <div class="wrap">
    <div class="logo">fala<span>real</span></div>
    <div class="nav-right">
      <div class="lang-toggle" role="group" aria-label="Escolher idioma">
        <button type="button" class="active" data-lang-btn="de">🇩🇪 Alemão</button>
        <button type="button" data-lang-btn="en">🇬🇧 Inglês</button>
      </div>
      <a href="#comecar" class="nav-cta">Quero testar</a>
    </div>
  </div>
</nav>

<header class="hero">
  <div class="wrap">
    <div class="hero-top">
      <div class="hero-text">
        <div class="lang-de">
          <span class="eyebrow">Pra brasileiro que vive (ou vai viver) na Alemanha</span>
          <h1>O alemão que te ensinam pra prova. <em>Nicht was dir die Realität zeigt, sondern was dir die Wahrheit gibt.</em></h1>
          <p class="sub">A maioria dos cursos te ensina um alemão de sala de aula — devagar, claro, sempre educado. A vida aqui não é assim. Aqui você treina alemão de verdade: pra se envolver de verdade — no trabalho, na consulta médica, na entrevista de emprego — com sotaque bávaro, suábio ou suíço, barulho ao fundo e gente te cortando no meio da frase.</p>
        </div>
        <div class="lang-en">
          <span class="eyebrow">Prática de conversação em inglês</span>
          <h1>O inglês que te preparam pra prova. <em>Não o que te deixa se envolver de verdade.</em></h1>
          <p class="sub">A maioria dos apps te ensina um inglês de laboratório — devagar, claro, sem interrupção. A vida real não é assim. Aqui você treina inglês de verdade: pra se envolver de verdade — no trabalho, viajando, ou vivendo fora — com sotaque, ruído e gente te cortando no meio da frase.</p>
        </div>
        <div class="hero-actions">
          <a href="#comecar" class="btn-primary">Quero testar agora</a>
          <a href="#niveis" class="btn-ghost">ver os 4 níveis ↓</a>
        </div>
      </div>

      <div class="hero-visual" aria-hidden="true">
        <svg viewBox="0 0 480 480" xmlns="http://www.w3.org/2000/svg" class="hero-illustration-svg">
<path d="M 100 90 Q 250 240 320 420" fill="none" style="stroke:var(--line); stroke-width:2; stroke-dasharray:4 8;" />
<path d="M 48 40 H 162 A 18 18 0 0 1 180 58 V 92 A 18 18 0 0 1 162 110 H 48 A 18 18 0 0 1 30 92 V 58 A 18 18 0 0 1 48 40 Z" style="fill:var(--ink-soft); stroke:var(--teal); stroke-width:2;" opacity="0.50" class="bubble" />
<path d="M 50.0 75.0 L 52.8 75.4 L 55.5 75.9 L 58.2 76.4 L 61.0 77.0 L 63.8 77.5 L 66.5 78.0 L 69.2 78.5 L 72.0 78.8 L 74.8 78.9 L 77.5 78.9 L 80.2 78.8 L 83.0 78.4 L 85.8 77.9 L 88.5 77.3 L 91.2 76.5 L 94.0 75.6 L 96.8 74.7 L 99.5 73.8 L 102.2 72.9 L 105.0 72.1 L 107.8 71.4 L 110.5 70.8 L 113.2 70.4 L 116.0 70.2 L 118.8 70.2 L 121.5 70.4 L 124.2 70.8 L 127.0 71.3 L 129.8 71.9 L 132.5 72.6 L 135.2 73.3 L 138.0 74.1 L 140.8 74.8 L 143.5 75.4 L 146.2 76.0 L 149.0 76.4 L 151.8 76.7 L 154.5 76.9 L 157.2 77.0 L 160.0 76.9" fill="none" style="stroke:var(--teal); stroke-width:3; stroke-linecap:round; stroke-linejoin:round;" />
<path d="M 158 130 H 302 A 18 18 0 0 1 320 148 V 192 A 18 18 0 0 1 302 210 H 158 A 18 18 0 0 1 140 192 V 148 A 18 18 0 0 1 158 130 Z" style="fill:var(--ink-soft); stroke:var(--teal); stroke-width:2;" opacity="0.62" class="bubble" />
<path d="M 160.0 170.0 L 163.5 171.1 L 167.0 172.4 L 170.5 173.6 L 174.0 174.8 L 177.5 175.6 L 181.0 176.0 L 184.5 175.9 L 188.0 175.2 L 191.5 174.0 L 195.0 172.3 L 198.5 170.2 L 202.0 168.0 L 205.5 165.8 L 209.0 163.9 L 212.5 162.3 L 216.0 161.4 L 219.5 161.2 L 223.0 161.7 L 226.5 162.9 L 230.0 164.7 L 233.5 167.0 L 237.0 169.4 L 240.5 171.9 L 244.0 174.2 L 247.5 176.1 L 251.0 177.4 L 254.5 178.0 L 258.0 178.0 L 261.5 177.3 L 265.0 176.0 L 268.5 174.4 L 272.0 172.5 L 275.5 170.6 L 279.0 168.9 L 282.5 167.4 L 286.0 166.4 L 289.5 165.8 L 293.0 165.7 L 296.5 166.0 L 300.0 166.6" fill="none" style="stroke:var(--teal); stroke-width:3; stroke-linecap:round; stroke-linejoin:round;" />
<path d="M 108 240 H 282 A 18 18 0 0 1 300 258 V 312 A 18 18 0 0 1 282 330 H 108 A 18 18 0 0 1 90 312 V 258 A 18 18 0 0 1 108 240 Z" style="fill:var(--ink-soft); stroke:var(--amber); stroke-width:2;" opacity="0.74" class="bubble" />
<path d="M 110.0 285.0 L 114.2 287.7 L 118.5 290.4 L 122.8 292.6 L 127.0 293.8 L 131.2 293.4 L 135.5 291.4 L 139.8 288.0 L 144.0 283.6 L 148.2 279.0 L 152.5 275.0 L 156.8 272.5 L 161.0 272.0 L 165.2 273.7 L 169.5 277.5 L 173.8 282.8 L 178.0 288.6 L 182.2 294.0 L 186.5 298.0 L 190.8 299.9 L 195.0 299.3 L 199.2 296.2 L 203.5 291.3 L 207.8 285.5 L 212.0 279.6 L 216.2 274.9 L 220.5 272.0 L 224.8 271.3 L 229.0 273.0 L 233.2 276.5 L 237.5 281.2 L 241.8 286.1 L 246.0 290.4 L 250.2 293.5 L 254.5 294.8 L 258.8 294.3 L 263.0 292.4 L 267.2 289.6 L 271.5 286.4 L 275.8 283.5 L 280.0 281.5" fill="none" style="stroke:var(--amber); stroke-width:3; stroke-linecap:round; stroke-linejoin:round;" />
<path d="M 178 350 H 382 A 18 18 0 0 1 400 368 V 432 A 18 18 0 0 1 382 450 H 178 A 18 18 0 0 1 160 432 V 368 A 18 18 0 0 1 178 350 Z" style="fill:var(--ink-soft); stroke:var(--rust); stroke-width:2;" opacity="0.86" class="bubble bubble-loud" />
<path d="M 180.0 400.0 L 185.0 405.7 L 190.0 410.7 L 195.0 412.9 L 200.0 410.8 L 205.0 404.7 L 210.0 396.0 L 215.0 387.5 L 220.0 382.3 L 225.0 382.4 L 230.0 388.4 L 235.0 398.7 L 240.0 410.2 L 245.0 419.2 L 250.0 422.4 L 255.0 418.5 L 260.0 408.6 L 265.0 395.6 L 270.0 383.7 L 275.0 376.8 L 280.0 377.2 L 285.0 384.7 L 290.0 397.0 L 295.0 410.0 L 300.0 419.7 L 305.0 422.9 L 310.0 418.9 L 315.0 409.3 L 320.0 397.3 L 325.0 386.9 L 330.0 381.2 L 335.0 381.6 L 340.0 387.6 L 345.0 396.8 L 350.0 405.9 L 355.0 412.2 L 360.0 414.0 L 365.0 411.4 L 370.0 405.7 L 375.0 399.3 L 380.0 394.4" fill="none" style="stroke:var(--rust); stroke-width:3; stroke-linecap:round; stroke-linejoin:round;" />
<g class="burst">
<line x1="404.0" y1="360.0" x2="420.0" y2="360.0" style="stroke:var(--rust); stroke-width:2; stroke-linecap:round;" opacity="0.7" />
<line x1="399.9" y1="369.9" x2="411.2" y2="381.2" style="stroke:var(--rust); stroke-width:2; stroke-linecap:round;" opacity="0.7" />
<line x1="390.0" y1="374.0" x2="390.0" y2="390.0" style="stroke:var(--rust); stroke-width:2; stroke-linecap:round;" opacity="0.7" />
<line x1="380.1" y1="369.9" x2="368.8" y2="381.2" style="stroke:var(--rust); stroke-width:2; stroke-linecap:round;" opacity="0.7" />
<line x1="376.0" y1="360.0" x2="360.0" y2="360.0" style="stroke:var(--rust); stroke-width:2; stroke-linecap:round;" opacity="0.7" />
<line x1="380.1" y1="350.1" x2="368.8" y2="338.8" style="stroke:var(--rust); stroke-width:2; stroke-linecap:round;" opacity="0.7" />
<line x1="390.0" y1="346.0" x2="390.0" y2="330.0" style="stroke:var(--rust); stroke-width:2; stroke-linecap:round;" opacity="0.7" />
<line x1="399.9" y1="350.1" x2="411.2" y2="338.8" style="stroke:var(--rust); stroke-width:2; stroke-linecap:round;" opacity="0.7" />
</g>
</svg>
      </div>
    </div>

    <div class="wave-stage" data-reveal>
      <div class="wave-labels">
        <span>nível 1 — devagar e claro</span>
        <span>nível 2</span>
        <span>nível 3</span>
        <span class="active">nível 4 — real</span>
      </div>
      <svg id="wave" viewBox="0 0 800 110" preserveAspectRatio="none"></svg>
      <p class="wave-caption">↑ cada nível soma sotaque, velocidade e ruído de fundo — igual ao mundo real</p>
    </div>
  </div>
</header>

<section id="comparacao">
  <div class="wrap">
    <div class="lang-de">
      <div class="section-head" data-reveal>
        <span class="kicker">O problema</span>
        <h2>Você já treinou isso. Só que nunca vai usar assim.</h2>
        <p class="lede">Volkshochschule, Duolingo e a maioria dos cursos treinam pra um alemão de livro que não existe no Amt, no consultório ou no trabalho. Aqui a diferença é o que acontece quando o funcionário fala rápido, tem sotaque forte, ou te corta no meio da frase.</p>
      </div>
      <div class="compare" data-reveal>
        <div class="lab">
          <h3>Curso de alemão</h3>
          <ul>
            <li>Alemão de livro, sempre educado</li>
            <li>Só Hochdeutsch neutro</li>
            <li>Diálogo decorado, sempre o mesmo</li>
            <li>Ninguém te apressa ou te corta</li>
            <li>Silêncio total ao fundo</li>
          </ul>
        </div>
        <div class="real">
          <h3>Fala Real</h3>
          <ul>
            <li>Alemão do dia a dia — trabalho, médico, vizinho, tudo</li>
            <li>Sotaque bávaro, suábio, saxão, suíço, austríaco</li>
            <li>Cenário novo a cada conversa</li>
            <li>Fila, pressa, gente te cortando</li>
            <li>Ruído de sala de espera, escritório, rua</li>
          </ul>
        </div>
      </div>
    </div>

    <div class="lang-en">
      <div class="section-head" data-reveal>
        <span class="kicker">O problema</span>
        <h2>Você já treinou isso. Só que nunca vai usar assim.</h2>
        <p class="lede">Duolingo, Babbel e a maioria dos apps treinam pra um inglês que não existe fora do aplicativo. Aqui a diferença é o que acontece quando alguém fala rápido, corta sua frase, ou tem um sotaque que você nunca ouviu.</p>
      </div>
      <div class="compare" data-reveal>
        <div class="lab">
          <h3>App de laboratório</h3>
          <ul>
            <li>Voz sintética, ritmo perfeito</li>
            <li>Um sotaque só, sempre o mesmo</li>
            <li>Silêncio total ao fundo</li>
            <li>A pessoa espera você terminar</li>
            <li>Mesmo exercício se repete igual</li>
          </ul>
        </div>
        <div class="real">
          <h3>Fala Real</h3>
          <ul>
            <li>Fala humana, com hesitação e ritmo real</li>
            <li>Vários sotaques, à sua escolha</li>
            <li>Rua, café, escritório, trânsito</li>
            <li>Interrupções e sobreposição de fala</li>
            <li>Cenário novo a cada conversa</li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</section>

<section id="niveis">
  <div class="wrap">
    <div class="section-head" data-reveal>
      <span class="kicker">O coração do produto</span>
      <h2>Quatro níveis. Cada um te tira um pouco mais da zona de conforto.</h2>
      <p class="lede">Você escolhe onde entrar e sobe no seu ritmo. Não é dificuldade por dificuldade — é uma progressão pensada pra chegar no dia a dia real.</p>
    </div>

    <div class="levels lang-de" data-reveal>
      <div class="level-row" data-level="1">
        <div class="level-num">01</div>
        <div>
          <div class="level-title">Devagar e claro</div>
          <p class="level-desc">Fala pausada, Hochdeutsch neutro, vocabulário do dia a dia. Ideal pra quem está destravando o ouvido de novo.</p>
          <div class="level-tags"><span>ritmo lento</span><span>sem ruído</span><span>Hochdeutsch neutro</span></div>
          <button class="level-audio-btn">🔊 Ouvir exemplo</button>
        </div>
      </div>
      <div class="level-row" data-level="2">
        <div class="level-num">02</div>
        <div>
          <div class="level-title">Ritmo do dia a dia</div>
          <p class="level-desc">A conversa já flui em velocidade real — supermercado, trabalho, vizinho no corredor.</p>
          <div class="level-tags"><span>ritmo normal</span><span>expressões do dia a dia</span><span>2 sotaques leves</span></div>
          <button class="level-audio-btn">🔊 Ouvir exemplo</button>
        </div>
      </div>
      <div class="level-row" data-level="3">
        <div class="level-num">03</div>
        <div>
          <div class="level-title">Sotaques e ambiente</div>
          <p class="level-desc">Sotaque bávaro, suábio ou saxão entram em cena, com ruído de fundo — sala de espera, café, escritório.</p>
          <div class="level-tags"><span>vários sotaques</span><span>ruído leve (Amt, café)</span></div>
          <button class="level-audio-btn">🔊 Ouvir exemplo</button>
        </div>
      </div>
      <div class="level-row" data-level="4">
        <div class="level-num">04</div>
        <div>
          <div class="level-title">Alemanha real</div>
          <p class="level-desc">Fila apertada, gente apressada, alemão suíço quase incompreensível, alguém te cortando no meio da frase.</p>
          <div class="level-tags"><span>interrupções</span><span>ruído forte</span><span>sotaques fortes (suíço, austríaco)</span></div>
          <button class="level-audio-btn">🔊 Ouvir exemplo (com interrupção)</button>
        </div>
      </div>
    </div>

    <div class="levels lang-en" data-reveal>
      <div class="level-row" data-level="1">
        <div class="level-num">01</div>
        <div>
          <div class="level-title">Devagar e claro</div>
          <p class="level-desc">Fala pausada, vocabulário direto, um sotaque neutro. Ideal pra quem está começando a treinar o ouvido de novo.</p>
          <div class="level-tags"><span>ritmo lento</span><span>sem ruído</span><span>1 sotaque</span></div>
          <button class="level-audio-btn">🔊 Ouvir exemplo</button>
        </div>
      </div>
      <div class="level-row" data-level="2">
        <div class="level-num">02</div>
        <div>
          <div class="level-title">Ritmo natural</div>
          <p class="level-desc">A conversa já flui em velocidade real, com contrações e gírias comuns do dia a dia.</p>
          <div class="level-tags"><span>ritmo normal</span><span>gírias leves</span><span>2 sotaques</span></div>
          <button class="level-audio-btn">🔊 Ouvir exemplo</button>
        </div>
      </div>
      <div class="level-row" data-level="3">
        <div class="level-num">03</div>
        <div>
          <div class="level-title">Sotaques e ambiente</div>
          <p class="level-desc">Sotaques variados entram em cena, com som de ambiente ao fundo — café, escritório, rua.</p>
          <div class="level-tags"><span>vários sotaques</span><span>ruído leve</span></div>
          <button class="level-audio-btn">🔊 Ouvir exemplo</button>
        </div>
      </div>
      <div class="level-row" data-level="4">
        <div class="level-num">04</div>
        <div>
          <div class="level-title">Rua real</div>
          <p class="level-desc">Interrupções, gente falando ao mesmo tempo, ruído de fundo forte. O mais perto que um app chega de uma conversa de verdade.</p>
          <div class="level-tags"><span>interrupções</span><span>ruído forte</span><span>sotaques fortes</span></div>
          <button class="level-audio-btn">🔊 Ouvir exemplo (com interrupção)</button>
        </div>
      </div>
    </div>
  </div>
</section>

<section id="experimente">
  <div class="wrap">
    <div class="section-head" data-reveal>
      <span class="kicker">Não seria justo só contar</span>
      <h2>Testa aqui. Os níveis não têm fim.</h2>
      <p class="lede">No app de verdade a dificuldade nunca para de subir, e você ganha por treinar todo dia. Duas mostras rápidas de como isso funciona:</p>
    </div>

    <div class="demo-grid" data-reveal>
      <div class="demo-card">
        <h3>Nível infinito</h3>
        <p class="demo-sub">Cada clique soma um elemento novo de dificuldade — sotaque, ruído, interrupção. Vai até onde você aguentar.</p>

        <div class="level-display">
          <div class="level-badge" id="level-badge">Nível 1</div>
          <div class="level-tier" id="level-tier">iniciante</div>
        </div>
        <div class="level-tags-live" id="level-tags"></div>

        <div class="mini-wave-wrap">
          <svg id="mini-wave" viewBox="0 0 400 60" preserveAspectRatio="none"></svg>
        </div>

        <div class="audio-row">
          <button class="btn-audio" id="listen-btn">🔊 Ouvir este nível</button>
          <span class="audio-status" id="audio-status"></span>
        </div>

        <button class="btn-primary btn-full" id="level-up-btn">Subir de nível ↑</button>
      </div>

      <div class="demo-card">
        <h3>Sequência diária</h3>
        <p class="demo-sub">Treina todo dia, mantém a sequência viva e destrava recompensas. Isso aqui já guarda seu progresso.</p>

        <div class="streak-hero">
          <span class="flame" id="flame">🔥</span>
          <div>
            <div class="streak-num" id="streak-num">0</div>
            <div class="streak-label">dias seguidos</div>
          </div>
        </div>

        <div class="streak-dots" id="streak-dots"></div>

        <div class="xp-row">
          <div class="xp-bar-track"><div class="xp-bar-fill" id="xp-fill"></div></div>
          <span class="xp-label" id="xp-label">0 xp</span>
        </div>

        <button class="btn-primary btn-full" id="streak-btn">Marcar hoje ✓</button>
        <div class="reward-toast" id="reward-toast"></div>

        <button class="btn-share" id="share-btn" style="display:none;">🎉 Compartilhar minha sequência</button>
        <div class="share-preview" id="share-preview" style="display:none;">
          <canvas id="share-canvas" width="1080" height="1080"></canvas>
          <div class="share-actions">
            <button class="btn-audio" id="download-share-btn">📥 Baixar imagem</button>
            <button class="btn-audio" id="whatsapp-share-btn">📲 Mandar no WhatsApp</button>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<section id="como-funciona">
  <div class="wrap">
    <div class="section-head" data-reveal>
      <span class="kicker">Como funciona</span>
      <h2>Simples de começar, difícil de decorar.</h2>
    </div>
    <div class="steps" data-reveal>
      <div class="step lang-de">
        <span class="n">passo 1</span>
        <h4>Você escolhe o cenário</h4>
        <p>Consulta médica, entrevista de emprego, conversa de vizinho — o cenário nunca se repete igual.</p>
      </div>
      <div class="step lang-en">
        <span class="n">passo 1</span>
        <h4>Você escolhe o cenário</h4>
        <p>Entrevista de emprego, pedido no restaurante, ligação de trabalho — o cenário nunca se repete igual.</p>
      </div>
      <div class="step">
        <span class="n">passo 2</span>
        <h4>Você conversa de verdade</h4>
        <p>Fala com a IA em tempo real, no nível de dificuldade que você escolheu.</p>
      </div>
      <div class="step">
        <span class="n">passo 3</span>
        <h4>Você recebe o retorno</h4>
        <p>O que você entendeu, o que passou batido, e o que treinar na próxima conversa.</p>
      </div>
    </div>
  </div>
</section>

<section id="preview">
  <div class="wrap">
    <div class="section-head" data-reveal>
      <span class="kicker">Um gostinho do produto</span>
      <h2>É mais ou menos assim que vai ficar.</h2>
      <p class="lede">Ainda estamos construindo, mas é isso que você vai ver na tela — uma conversa de verdade, com feedback na hora, não um exercício de múltipla escolha.</p>
    </div>

    <div class="phone-mockup-wrap" data-reveal>
      <div class="phone-frame">
        <div class="phone-notch"></div>

        <div class="lang-de">
          <div class="phone-topbar">
            <span class="phone-level-badge">Nível 3 · No dia a dia</span>
            <span class="phone-mic-status"><span class="dot"></span> ouvindo</span>
          </div>
          <div class="phone-chat">
            <div class="chat-bubble ai">Also, das Formular müssen Sie noch einmal ausfüllen, ja? Und den Ausweis nicht vergessen.</div>
            <div class="chat-bubble user">Äh... welche Formular genau?</div>
            <div class="chat-bubble feedback">✏️ Quase lá! Era <strong>"welches"</strong> Formular, não "welche". A pronúncia ficou ótima.</div>
          </div>
        </div>

        <div class="lang-en">
          <div class="phone-topbar">
            <span class="phone-level-badge">Level 3 · Job interview</span>
            <span class="phone-mic-status"><span class="dot"></span> listening</span>
          </div>
          <div class="phone-chat">
            <div class="chat-bubble ai">So you'll need to fill out that form again, yeah? And don't forget your ID.</div>
            <div class="chat-bubble user">Uh... which forms exactly?</div>
            <div class="chat-bubble feedback">✏️ Almost! It's <strong>"which form"</strong>, not "which forms" — pronunciation was great though.</div>
          </div>
        </div>

        <div class="phone-mic-btn"><span class="mic-pulse"></span><span class="mic-pulse mic-pulse-2"></span>🎙️</div>
      </div>
    </div>
  </div>
</section>

<section id="diagnostico">
  <div class="wrap">
    <div class="section-head" data-reveal>
      <span class="kicker">30 segundos</span>
      <h2>Antes de continuar, me conta uma coisa.</h2>
      <p class="lede">Duas perguntas rápidas pra eu te indicar por onde começar — sem compromisso nenhum.</p>
    </div>

    <div class="quiz-card" data-reveal>
      <!-- Passo 1 -->
      <div class="quiz-step active" data-step="1">
        <div class="lang-de"><p class="quiz-question">Qual é o seu maior desafio hoje?</p></div>
        <div class="lang-en"><p class="quiz-question">What's your biggest challenge right now?</p></div>

        <div class="quiz-options lang-de">
          <button class="quiz-option" data-key="sotaque" data-label="Entender sotaque forte">Entender sotaque forte</button>
          <button class="quiz-option" data-key="envolvimento" data-label="Se envolver de verdade (comunidade, dia a dia)">Se envolver de verdade (comunidade, dia a dia)</button>
          <button class="quiz-option" data-key="entrevista" data-label="Entrevista de emprego">Entrevista de emprego</button>
          <button class="quiz-option" data-key="trabalho" data-label="Conversar no trabalho">Conversar no trabalho</button>
        </div>
        <div class="quiz-options lang-en">
          <button class="quiz-option" data-key="sotaque" data-label="Understanding strong accents">Understanding strong accents</button>
          <button class="quiz-option" data-key="envolvimento" data-label="Getting truly involved (community, daily life)">Getting truly involved (community, daily life)</button>
          <button class="quiz-option" data-key="entrevista" data-label="Job interviews">Job interviews</button>
          <button class="quiz-option" data-key="trabalho" data-label="Everyday work conversation">Everyday work conversation</button>
        </div>
      </div>

      <!-- Passo 2 -->
      <div class="quiz-step" data-step="2">
        <div class="lang-de"><p class="quiz-question">Como está seu alemão hoje?</p></div>
        <div class="lang-en"><p class="quiz-question">How's your English today?</p></div>

        <div class="quiz-options lang-de">
          <button class="quiz-option" data-key="1" data-label="Iniciante total">Iniciante total</button>
          <button class="quiz-option" data-key="2" data-label="Me viro no básico">Me viro no básico</button>
          <button class="quiz-option" data-key="3" data-label="Intermediário, mas travo no sotaque">Intermediário, mas travo no sotaque</button>
        </div>
        <div class="quiz-options lang-en">
          <button class="quiz-option" data-key="1" data-label="Total beginner">Total beginner</button>
          <button class="quiz-option" data-key="2" data-label="I get by with the basics">I get by with the basics</button>
          <button class="quiz-option" data-key="3" data-label="Intermediate, but accents trip me up">Intermediate, but accents trip me up</button>
        </div>
      </div>

      <!-- Resultado -->
      <div class="quiz-step" data-step="result">
        <div class="quiz-result-icon">🎯</div>
        <div class="lang-de">
          <p class="quiz-result-title">Nível sugerido pra você: <span id="quiz-level-de">2</span></p>
          <p class="quiz-result-desc" id="quiz-desc-de">Baseado no que você respondeu, sugerimos focar em se envolver de verdade na vida daqui.</p>
        </div>
        <div class="lang-en">
          <p class="quiz-result-title">Suggested level for you: <span id="quiz-level-en">2</span></p>
          <p class="quiz-result-desc" id="quiz-desc-en">Based on your answers, we'd suggest focusing on bureaucracy scenarios.</p>
        </div>
        <a href="#comecar" class="btn-primary" id="quiz-cta-btn">Continuar pra lista de espera ↓</a>
      </div>

      <div class="quiz-progress">
        <span class="quiz-dot active" data-dot="1"></span>
        <span class="quiz-dot" data-dot="2"></span>
        <span class="quiz-dot" data-dot="result"></span>
      </div>
    </div>
  </div>
</section>

<section class="cta-band" id="comecar">
  <div class="wrap">
    <div class="cta-inner lang-de" data-reveal>
      <span class="kicker">Fase inicial</span>
      <h2>Estamos abrindo pras primeiras pessoas — brasileiros na Alemanha — agora.</h2>
      <p class="lede">Deixa seu e-mail que a gente te chama assim que abrir uma vaga pra testar — e você ajuda a decidir os próximos cenários, do trabalho ao dia a dia.</p>
      <p class="quiz-summary" id="quiz-summary-de"></p>
      <form class="email-form" id="waitlist-form-de">
        <input type="email" name="email" required placeholder="seu@email.com" aria-label="Seu e-mail">
        <input type="hidden" name="desafio" id="quiz-desafio-de">
        <input type="hidden" name="nivel_percebido" id="quiz-nivel-de">
        <input type="hidden" name="indicado_por" id="ref-de">
        <button type="submit" class="btn-primary">Quero entrar na lista</button>
      </form>
      <p class="form-note">sem spam — só um e-mail quando abrir sua vaga</p>
      <div class="thanks" id="thanks-msg-de">
        <p>Prontinho! Assim que abrir uma vaga, você é uma das primeiras pessoas a saber.</p>
        <div class="referral-box">
          <p class="referral-title">🚀 Quer subir na fila? Convide amigos.</p>
          <p class="referral-desc">Quem entrar pelo seu link — e você — sobem juntos pra acesso prioritário.</p>
          <div class="referral-link-row">
            <input type="text" readonly id="referral-link-de" class="referral-input">
            <button class="btn-audio" id="copy-referral-de">📋 Copiar</button>
          </div>
          <button class="btn-share" id="whatsapp-referral-de">📲 Convidar no WhatsApp</button>
        </div>
      </div>
    </div>

    <div class="cta-inner lang-en" data-reveal>
      <span class="kicker">Fase inicial</span>
      <h2>Estamos abrindo pras primeiras pessoas agora.</h2>
      <p class="lede">Deixa seu e-mail que a gente te chama assim que abrir uma vaga pra testar — e você ajuda a moldar o produto antes de todo mundo.</p>
      <p class="quiz-summary" id="quiz-summary-en"></p>
      <form class="email-form" id="waitlist-form-en">
        <input type="email" name="email" required placeholder="seu@email.com" aria-label="Seu e-mail">
        <input type="hidden" name="desafio" id="quiz-desafio-en">
        <input type="hidden" name="nivel_percebido" id="quiz-nivel-en">
        <input type="hidden" name="indicado_por" id="ref-en">
        <button type="submit" class="btn-primary">Quero entrar na lista</button>
      </form>
      <p class="form-note">sem spam — só um e-mail quando abrir sua vaga</p>
      <div class="thanks" id="thanks-msg-en">
        <p>Prontinho! Assim que abrir uma vaga, você é uma das primeiras pessoas a saber.</p>
        <div class="referral-box">
          <p class="referral-title">🚀 Quer subir na fila? Convide amigos.</p>
          <p class="referral-desc">Quem entrar pelo seu link — e você — sobem juntos pra acesso prioritário.</p>
          <div class="referral-link-row">
            <input type="text" readonly id="referral-link-en" class="referral-input">
            <button class="btn-audio" id="copy-referral-en">📋 Copiar</button>
          </div>
          <button class="btn-share" id="whatsapp-referral-en">📲 Convidar no WhatsApp</button>
        </div>
      </div>
    </div>
  </div>
</section>

<footer>
  <div class="wrap">
    <div class="logo">fala<span>real</span> <span class="version-tag">v11.0.0</span></div>
    <p class="lang-de">Feito por um brazuca que já viveu mais de 6 anos na Alemanha.</p>
    <p class="lang-en">feito pra quem já cansou do inglês de laboratório</p>
  </div>
</footer>

<script>
  // Reveal on scroll
  const revealEls = document.querySelectorAll('[data-reveal]');
  const io = new IntersectionObserver((entries)=>{
    entries.forEach(e=>{ if(e.isIntersecting){ e.target.classList.add('in'); io.unobserve(e.target); } });
  }, {threshold:0.15});
  revealEls.forEach(el=>io.observe(el));

  // Waveform: calm on the left, chaotic/noisy on the right (mirrors the 4 levels)
  const svgNS = "http://www.w3.org/2000/svg";
  const wave = document.getElementById('wave');
  const W = 800, H = 110, MID = H/2;
  const bars = 80;
  const barEls = [];
  for(let i=0;i<bars;i++){
    const x = (i/bars)*W;
    const rect = document.createElementNS(svgNS,'rect');
    rect.setAttribute('x', x);
    rect.setAttribute('width', (W/bars)*0.6);
    rect.setAttribute('rx', 2);
    const t = i/bars; // 0 = calm, 1 = chaotic
    const color = t < 0.33 ? '#3e6b63' : t < 0.66 ? '#f0a63a' : '#c1483d';
    rect.setAttribute('fill', color);
    rect.setAttribute('opacity', 0.85);
    wave.appendChild(rect);
    barEls.push({rect, t, x});
  }

  let frame = 0;
  function animate(){
    frame += 1;
    barEls.forEach(({rect,t,x}, i)=>{
      const chaos = 0.15 + t*1.4; // more chaotic further right
      const speed = 0.05 + t*0.18;
      const noise = Math.sin(frame*speed + i*0.5) * (18 + t*40) + Math.sin(frame*speed*1.7 + i) * (6 + t*20*chaos);
      const h = Math.max(4, Math.abs(noise) + 6);
      rect.setAttribute('y', MID - h/2);
      rect.setAttribute('height', h);
    });
    requestAnimationFrame(animate);
  }
  animate();

  // ---- IDIOMA ----
  let currentLang = 'de';
  const langButtons = document.querySelectorAll('[data-lang-btn]');
  langButtons.forEach(btn=>{
    btn.addEventListener('click', ()=>{
      currentLang = btn.getAttribute('data-lang-btn');
      document.body.classList.remove('lang-de','lang-en');
      document.body.classList.add('lang-' + currentLang);
      langButtons.forEach(b=>b.classList.toggle('active', b === btn));
      if(typeof stopAllAudio === 'function') stopAllAudio();
      renderLevel(currentLevel);
    });
  });

  // ---- NÍVEL INFINITO ----
  const contentByLang = {
    de: {
      accents: ['sotaque bávaro fechado','sotaque suábio cantado','sotaque saxão (Sächsisch)','alemão suíço quase incompreensível','sotaque austríaco','sotaque berlinense debochado','sotaque do Ruhrgebiet','alemão com forte influência turca da rua'],
      noises: ['sala de espera do médico lotada','fila enorme no guichê do Amt','Biergarten cheio no verão','U-Bahn na hora do rush','obra do lado do apartamento','festa de rua com música alta','padaria lotada de manhã','escritório aberto e barulhento'],
      interrupts: ['o funcionário do Amt te corta e pede outro documento','o médico fala rápido demais e já muda de assunto','a call em alemão cai bem na hora H','o colega de trabalho fala rápido e usa gíria','duas pessoas discutindo ao mesmo tempo no guichê','o atendente te apressa pra decidir na hora'],
      phrases: ['Guten Tag, wie kann ich Ihnen helfen?','Ich brauche einen Termin für nächste Woche, wenn möglich.','Entschuldigung, könnten Sie das bitte langsamer wiederholen?','Also, wir haben da noch ein Formular, das fehlt noch, ne?','Moment mal, ich hab Sie nicht ganz verstanden.','Das geht heute leider nicht mehr, der nächste Termin ist erst im März.'],
      audioFiles: ['audio/de-phrase1.mp3','audio/de-phrase2.mp3','audio/de-phrase3.mp3','audio/de-phrase4.mp3','audio/de-phrase5.mp3','audio/de-phrase6.mp3'],
      voiceLocales: ['de-DE','de-AT','de-CH','de-DE','de-AT','de-DE']
    },
    en: {
      accents: ['sotaque escocês fechado','sotaque australiano arrastado','sotaque indiano acelerado','sotaque texano puxado','sotaque irlandês cantado','sotaque nigeriano firme','sotaque cockney de Londres','sotaque cajun da Louisiana','sotaque sul-africano','sotaque de Boston'],
      noises: ['trânsito buzinando','café lotado no horário de pico','vento forte no telefone','festa no fundo','obra na rua do lado','multidão no metrô','TV ligada alto na sala','crianças gritando por perto','chuva forte no telhado','bar cheio no fim de semana'],
      interrupts: ['o outro corta sua frase no meio','duas pessoas falando ao mesmo tempo','a call cai bem na hora H','o atendente te apressa pra decidir','o garçom interrompe o pedido','alguém grita seu nome no meio da frase','o sinal corta por 2 segundos'],
      phrases: ['Hi there, how can I help you today?','I need an appointment for next week if possible.','Sorry, could you say that again a bit slower?','Yeah so we still need that form before we can process this.','Hang on, I didn\'t quite catch that.','That won\'t work today, the next slot is in March.'],
      audioFiles: ['audio/en-phrase1.mp3','audio/en-phrase2.mp3','audio/en-phrase3.mp3','audio/en-phrase4.mp3','audio/en-phrase5.mp3','audio/en-phrase6.mp3'],
      voiceLocales: ['en-US','en-GB','en-AU','en-IN','en-ZA','en-IE','en-US','en-GB']
    }
  };
  const tiers = ['iniciante','confortável','desafiador','intenso','brutal','insano','lendário'];

  let currentLevel = 1;
  const levelBadge = document.getElementById('level-badge');
  const levelTier = document.getElementById('level-tier');
  const levelTags = document.getElementById('level-tags');
  const levelUpBtn = document.getElementById('level-up-btn');

  function pick(list, seed){ return list[seed % list.length]; }

  function renderLevel(n){
    levelBadge.textContent = 'Nível ' + n;
    const tierIndex = Math.min(Math.floor((n-1)/3), tiers.length-1);
    levelTier.textContent = tiers[tierIndex] + (n > tiers.length*3 ? ' +' : '');

    const elementCount = n <= 3 ? 1 : n <= 7 ? 2 : n <= 15 ? 3 : 4;
    const lists = contentByLang[currentLang];
    const pool = [];
    pool.push(pick(lists.accents, n));
    if(elementCount >= 2) pool.push(pick(lists.noises, n+2));
    if(elementCount >= 3) pool.push(pick(lists.interrupts, n+4));
    if(elementCount >= 4) pool.push(pick(lists.noises, n+7));

    levelTags.innerHTML = '';
    pool.forEach(txt=>{
      const span = document.createElement('span');
      span.textContent = txt;
      levelTags.appendChild(span);
    });

    // color badge hotter as level rises
    const heat = Math.min(n/20, 1);
    const r = Math.round(240 + heat*(193-240));
    const g = Math.round(166 + heat*(72-166));
    const b = Math.round(58 + heat*(61-58));
    levelBadge.style.color = `rgb(${r},${g},${b})`;

    renderMiniWave(n);
  }

  levelUpBtn.addEventListener('click', ()=>{
    if(typeof stopAllAudio === 'function') stopAllAudio();
    currentLevel += 1;
    renderLevel(currentLevel);
  });

  // ---- MOTOR DE ÁUDIO: ruído de fundo (Web Audio API) + voz sintetizada (Speech Synthesis) ----
  const listenBtn = document.getElementById('listen-btn');
  const audioStatus = document.getElementById('audio-status');
  let audioCtx = null;
  let noiseNodes = null;
  let voicesCache = [];
  let activeAudioBtn = null;

  function loadVoices(){
    voicesCache = window.speechSynthesis ? window.speechSynthesis.getVoices() : [];
  }
  if(window.speechSynthesis){
    loadVoices();
    window.speechSynthesis.onvoiceschanged = loadVoices;
  }

  function pickVoice(locale){
    if(!voicesCache.length) return null;
    const family = locale.split('-')[0];
    const matches = voicesCache.filter(v => v.lang === locale || (v.lang && v.lang.startsWith(family)));
    if(!matches.length) return null;

    // prefer exact locale match over just same language family
    const exact = matches.filter(v => v.lang === locale);
    const pool = exact.length ? exact : matches;

    // score voices: network/cloud engines and "natural"-labelled voices sound far less robotic
    // than compact on-device ones, so push those to the front when available
    const scored = pool.map(v=>{
      let score = 0;
      if(v.localService === false) score += 3;          // cloud voice (usually Google's, much better)
      if(/google/i.test(v.name)) score += 2;
      if(/natural|neural|enhanced|premium|online/i.test(v.name)) score += 2;
      if(/compact|espeak|mobile/i.test(v.name)) score -= 2;
      return {v, score};
    }).sort((a,b)=> b.score - a.score);

    return scored[0].v;
  }

  function startNoise(chaos){
    try{
      audioCtx = audioCtx || new (window.AudioContext || window.webkitAudioContext)();
      if(audioCtx.state === 'suspended') audioCtx.resume();

      const bufferSize = audioCtx.sampleRate * 2;
      const buffer = audioCtx.createBuffer(1, bufferSize, audioCtx.sampleRate);
      const data = buffer.getChannelData(0);
      for(let i=0;i<bufferSize;i++){ data[i] = (Math.random()*2-1); }

      const noiseSource = audioCtx.createBufferSource();
      noiseSource.buffer = buffer;
      noiseSource.loop = true;

      const filter = audioCtx.createBiquadFilter();
      filter.type = 'bandpass';
      filter.frequency.value = 400 + chaos*900;
      filter.Q.value = 0.6;

      const gain = audioCtx.createGain();
      const targetGain = Math.min(0.02 + chaos*0.16, 0.24);
      gain.gain.setValueAtTime(0, audioCtx.currentTime);
      gain.gain.linearRampToValueAtTime(targetGain, audioCtx.currentTime + 0.4);

      noiseSource.connect(filter);
      filter.connect(gain);
      gain.connect(audioCtx.destination);
      noiseSource.start();

      noiseNodes = {noiseSource, gain};
    }catch(e){ noiseNodes = null; }
  }

  // pushes the noise louder for a moment — used to punctuate the interruption in level 4
  function surgeNoise(){
    if(!noiseNodes || !audioCtx) return;
    try{
      const { gain } = noiseNodes;
      const now = audioCtx.currentTime;
      gain.gain.cancelScheduledValues(now);
      gain.gain.setValueAtTime(gain.gain.value, now);
      gain.gain.linearRampToValueAtTime(Math.min(gain.gain.value + 0.14, 0.34), now + 0.15);
      gain.gain.linearRampToValueAtTime(Math.max(gain.gain.value - 0.05, 0.1), now + 1.2);
    }catch(e){}
  }

  function stopNoise(){
    if(!noiseNodes) return;
    try{
      const {noiseSource, gain} = noiseNodes;
      gain.gain.cancelScheduledValues(audioCtx.currentTime);
      gain.gain.linearRampToValueAtTime(0, audioCtx.currentTime + 0.3);
      setTimeout(()=>{ try{ noiseSource.stop(); }catch(e){} }, 350);
    }catch(e){}
    noiseNodes = null;
  }

  // stops whatever is currently playing (either widget) and resets its button
  function stopAllAudio(){
    if(window.speechSynthesis) window.speechSynthesis.cancel();
    if(activeAudioEl){ try{ activeAudioEl.pause(); }catch(e){} activeAudioEl = null; }
    stopNoise();
    if(activeAudioBtn){
      activeAudioBtn.classList.remove('playing');
      activeAudioBtn.disabled = false;
      activeAudioBtn.textContent = activeAudioBtn.dataset.defaultLabel;
      activeAudioBtn = null;
    }
    if(audioStatus) audioStatus.textContent = '';
  }

  // ---- Botão "Ouvir este nível" do simulador de nível infinito ----
  listenBtn.dataset.defaultLabel = '🔊 Ouvir este nível';
  listenBtn.addEventListener('click', ()=>{
    stopAllAudio();

    const n = currentLevel;
    const lists = contentByLang[currentLang];
    const elementCount = n <= 3 ? 1 : n <= 7 ? 2 : n <= 15 ? 3 : 4;
    const chaos = Math.min((elementCount-1)/3, 1);
    const locale = pick(lists.voiceLocales, n);
    const phrase = pick(lists.phrases, n);
    const rate = Math.min(0.85 + (n-1)*0.025, 1.4);

    activeAudioBtn = listenBtn;
    listenBtn.classList.add('playing');
    listenBtn.disabled = true;
    listenBtn.textContent = '🔊 Tocando...';
    audioStatus.textContent = locale;

    // usa o áudio real gravado quando existir pra essa mesma frase/idioma
    if(lists.audioFiles){
      const audioUrl = pick(lists.audioFiles, n);
      playRealAudio(audioUrl, chaos, stopAllAudio);
      return;
    }

    // reserva: voz do navegador (usada enquanto não temos áudio real pro idioma atual)
    if(!window.speechSynthesis){
      audioStatus.textContent = 'seu navegador não suporta áudio aqui';
      return;
    }
    if(chaos > 0) startNoise(chaos);

    setTimeout(()=>{
      const utter = new SpeechSynthesisUtterance(phrase);
      utter.lang = locale;
      utter.rate = rate;
      const voice = pickVoice(locale);
      if(voice) utter.voice = voice;

      utter.onend = stopAllAudio;
      utter.onerror = stopAllAudio;
      window.speechSynthesis.speak(utter);
    }, chaos > 0 ? 350 : 60);
  });

  // ---- Exemplos de áudio dos 4 níveis fixos ----
  // Se existir um arquivo real em REAL_AUDIO (gravado no ElevenLabs), ele toca em vez da voz do navegador.
  const REAL_AUDIO = {
    de: {
      1: 'audio/de-level1.mp3',
      2: 'audio/de-level2.mp3',
      3: 'audio/de-level3.mp3',
      4: 'audio/de-level4.mp3'
    },
    en: {
      1: 'audio/en-level1.mp3',
      2: 'audio/en-level2.mp3',
      3: 'audio/en-level3.mp3',
      4: 'audio/en-level4.mp3'
    }
  };
  const LEVEL_CHAOS = { 1:0, 2:0.3, 3:0.6, 4:0.95 };

  const LEVEL_DEMOS = {
    de: {
      1: { phrase:'Guten Tag, wie kann ich Ihnen helfen?', locale:'de-DE', rate:0.8, chaos:0 },
      2: { phrase:'Ich brauche einen Termin für nächste Woche, wenn möglich.', locale:'de-DE', rate:1.0, chaos:0.3 },
      3: { phrase:'Also, das Formular müssen Sie leider noch einmal ausfüllen, ja?', locale:'de-AT', rate:1.1, chaos:0.6 },
      4: { phrase:'Nein, warten Sie, das Dokument fehlt immer noch!', locale:'de-DE', rate:1.3, chaos:0.95 }
    },
    en: {
      1: { phrase:'Hi there, how can I help you today?', locale:'en-US', rate:0.8, chaos:0 },
      2: { phrase:'I need an appointment for next week if possible.', locale:'en-US', rate:1.0, chaos:0.3 },
      3: { phrase:"So you'll need to fill out that form again, yeah?", locale:'en-GB', rate:1.1, chaos:0.6 },
      4: { phrase:"No wait, hold on, that document's still missing!", locale:'en-US', rate:1.3, chaos:0.95 }
    }
  };

  let activeAudioEl = null;

  function playRealAudio(url, chaos, onDone){
    if(chaos > 0) startNoise(chaos);
    const audioEl = new Audio(url);
    activeAudioEl = audioEl;
    audioEl.addEventListener('ended', onDone);
    audioEl.addEventListener('error', onDone);
    // small head start so the noise is already under way when the voice comes in
    setTimeout(()=> audioEl.play().catch(onDone), chaos > 0 ? 300 : 0);
  }

  document.querySelectorAll('.level-audio-btn').forEach(btn=>{
    btn.dataset.defaultLabel = btn.textContent;
    btn.addEventListener('click', ()=>{
      stopAllAudio();

      const lang = btn.closest('.levels').classList.contains('lang-de') ? 'de' : 'en';
      const levelNum = parseInt(btn.closest('.level-row').getAttribute('data-level'), 10);
      const realUrl = REAL_AUDIO[lang] && REAL_AUDIO[lang][levelNum];

      activeAudioBtn = btn;
      btn.classList.add('playing');
      btn.disabled = true;
      btn.textContent = '🔊 Tocando...';

      if(realUrl){
        playRealAudio(realUrl, LEVEL_CHAOS[levelNum] || 0, stopAllAudio);
        return;
      }

      // reserva: voz do navegador, pra quando ainda não tem o áudio real desse nível/idioma
      if(!window.speechSynthesis){
        btn.textContent = 'sem suporte a áudio';
        return;
      }
      const cfg = LEVEL_DEMOS[lang][levelNum];
      if(!cfg) return;

      if(cfg.chaos > 0) startNoise(cfg.chaos);
      setTimeout(()=>{
        const u = new SpeechSynthesisUtterance(cfg.phrase);
        u.lang = cfg.locale; u.rate = cfg.rate;
        const v = pickVoice(cfg.locale); if(v) u.voice = v;
        u.onend = stopAllAudio;
        u.onerror = stopAllAudio;
        window.speechSynthesis.speak(u);
      }, cfg.chaos > 0 ? 350 : 60);
    });
  });

  // mini wave scales chaos with level, no visual cap on how high level can go
  const miniWave = document.getElementById('mini-wave');
  const miniBars = 40;
  const miniBarEls = [];
  for(let i=0;i<miniBars;i++){
    const rect = document.createElementNS(svgNS,'rect');
    rect.setAttribute('x', (i/miniBars)*400);
    rect.setAttribute('width', (400/miniBars)*0.6);
    rect.setAttribute('rx', 1.5);
    rect.setAttribute('fill', '#f0a63a');
    miniWave.appendChild(rect);
    miniBarEls.push(rect);
  }
  let miniLevel = 1;
  function renderMiniWave(n){ miniLevel = n; }
  let miniFrame = 0;
  function animateMini(){
    miniFrame += 1;
    const chaos = Math.min(miniLevel/12, 1.6);
    miniBarEls.forEach((rect,i)=>{
      const noise = Math.sin(miniFrame*(0.06+chaos*0.05) + i*0.6) * (6 + chaos*22);
      const h = Math.max(3, Math.abs(noise)+4);
      rect.setAttribute('y', 30 - h/2);
      rect.setAttribute('height', h);
    });
    requestAnimationFrame(animateMini);
  }
  renderLevel(currentLevel);
  animateMini();

  // ---- SEQUÊNCIA DIÁRIA ----
  const STORAGE_KEY = 'falareal_streak_v1';
  function todayStr(){ return new Date().toISOString().slice(0,10); }
  function daysBetween(a,b){ return Math.round((new Date(b) - new Date(a)) / 86400000); }

  function loadStreak(){
    try{
      const raw = localStorage.getItem(STORAGE_KEY);
      return raw ? JSON.parse(raw) : {streak:0, xp:0, lastDate:null};
    }catch(e){ return {streak:0, xp:0, lastDate:null}; }
  }
  function saveStreak(data){
    try{ localStorage.setItem(STORAGE_KEY, JSON.stringify(data)); }catch(e){}
  }

  let streakData = loadStreak();

  const streakNumEl = document.getElementById('streak-num');
  const streakDotsEl = document.getElementById('streak-dots');
  const xpFillEl = document.getElementById('xp-fill');
  const xpLabelEl = document.getElementById('xp-label');
  const flameEl = document.getElementById('flame');
  const streakBtn = document.getElementById('streak-btn');
  const rewardToast = document.getElementById('reward-toast');

  const milestones = [
    {days:3, label:'Sequência de bronze desbloqueada'},
    {days:7, label:'Sequência de prata desbloqueada'},
    {days:14, label:'Sequência de ouro desbloqueada'},
    {days:30, label:'Sequência lendária desbloqueada'}
  ];

  function renderStreak(){
    streakNumEl.textContent = streakData.streak;
    flameEl.classList.toggle('lit', streakData.streak > 0);

    streakDotsEl.innerHTML = '';
    const filled = Math.min(streakData.streak, 7);
    for(let i=0;i<7;i++){
      const d = document.createElement('div');
      d.className = 'dot' + (i < filled ? ' filled' : '');
      streakDotsEl.appendChild(d);
    }

    const xpForBar = streakData.xp % 100;
    xpFillEl.style.width = xpForBar + '%';
    xpLabelEl.textContent = streakData.xp + ' xp';

    const markedToday = streakData.lastDate === todayStr();
    streakBtn.textContent = markedToday ? 'Treinado hoje ✓' : 'Marcar hoje ✓';
    streakBtn.disabled = markedToday;
    streakBtn.style.opacity = markedToday ? '0.55' : '1';
    streakBtn.style.cursor = markedToday ? 'default' : 'pointer';

    if(streakData.streak > 0){
      document.getElementById('share-btn').style.display = 'block';
    }
  }

  streakBtn.addEventListener('click', ()=>{
    const today = todayStr();
    if(streakData.lastDate === today) return;

    if(streakData.lastDate){
      const gap = daysBetween(streakData.lastDate, today);
      streakData.streak = gap === 1 ? streakData.streak + 1 : 1;
    } else {
      streakData.streak = 1;
    }
    streakData.lastDate = today;
    streakData.xp += 10;
    saveStreak(streakData);
    renderStreak();

    const hit = milestones.find(m => m.days === streakData.streak);
    if(hit){
      rewardToast.textContent = '🏅 ' + hit.label;
      rewardToast.classList.add('show');
      confettiBurst();
    } else {
      rewardToast.textContent = '+10 xp — volta amanhã pra manter a sequência';
      rewardToast.classList.add('show');
    }
    setTimeout(()=> rewardToast.classList.remove('show'), 3200);
  });

  renderStreak();

  // ---- Confete (leve, sem biblioteca externa) ----
  function confettiBurst(){
    const colors = ['#f0a63a', '#3e6b63', '#c1483d', '#f4efe6'];
    const originX = window.innerWidth / 2;
    const originY = window.innerHeight * 0.35;
    for(let i=0;i<28;i++){
      const piece = document.createElement('div');
      piece.className = 'confetti-piece';
      piece.style.background = colors[i % colors.length];
      piece.style.left = originX + 'px';
      piece.style.top = originY + 'px';
      const drift = (Math.random()-0.5) * 500;
      const spin = (Math.random()>0.5 ? 1 : -1) * (360 + Math.random()*360);
      piece.style.setProperty('--drift', drift + 'px');
      piece.style.setProperty('--spin', spin + 'deg');
      piece.style.animation = `confetti-fall ${1.4 + Math.random()*0.8}s ease-in forwards`;
      document.body.appendChild(piece);
      setTimeout(()=> piece.remove(), 2400);
    }
  }

  // ---- Card de compartilhamento (Canvas, gerado na hora) ----
  const shareBtn = document.getElementById('share-btn');
  const sharePreview = document.getElementById('share-preview');
  const shareCanvas = document.getElementById('share-canvas');
  const downloadShareBtn = document.getElementById('download-share-btn');
  const whatsappShareBtn = document.getElementById('whatsapp-share-btn');

  function drawShareCard(){
    const ctx = shareCanvas.getContext('2d');
    const S = 1080;

    // fundo
    const grad = ctx.createLinearGradient(0,0,0,S);
    grad.addColorStop(0, '#1c2530');
    grad.addColorStop(1, '#12181f');
    ctx.fillStyle = grad;
    ctx.fillRect(0,0,S,S);

    // marca
    ctx.textBaseline = 'alphabetic';
    ctx.font = '600 64px Georgia, serif';
    ctx.fillStyle = '#f4efe6';
    ctx.fillText('fala', 90, 150);
    const falaWidth = ctx.measureText('fala').width;
    ctx.fillStyle = '#f0a63a';
    ctx.fillText('real', 90 + falaWidth, 150);

    // chama + número
    ctx.font = '260px sans-serif';
    ctx.fillText('🔥', 90, 480);

    ctx.font = '700 220px Georgia, serif';
    ctx.fillStyle = '#f4efe6';
    ctx.fillText(String(streakData.streak), 380, 470);

    ctx.font = '500 40px monospace';
    ctx.fillStyle = 'rgba(244,239,230,0.7)';
    const dayLabel = currentLang === 'de' ? 'TAGE IN FOLGE' : 'DIAS SEGUIDOS';
    ctx.fillText(dayLabel, 92, 560);

    // frase
    ctx.font = '38px monospace';
    ctx.fillStyle = '#f4efe6';
    const phrase = currentLang === 'de'
      ? 'Ich trainiere echtes Deutsch.'
      : 'Treinando alemão de verdade.';
    ctx.fillText(phrase, 92, 680);

    // waveform decorativa
    const barCount = 40;
    const barBaseX = 92, barY = 820, barMaxH = 90, barW = (S-184)/barCount;
    for(let i=0;i<barCount;i++){
      const t = i/barCount;
      ctx.fillStyle = t < 0.33 ? '#3e6b63' : t < 0.66 ? '#f0a63a' : '#c1483d';
      const h = 14 + Math.abs(Math.sin(i*0.8))*barMaxH*(0.3+t);
      ctx.beginPath();
      ctx.roundRect(barBaseX + i*barW, barY - h/2, barW*0.6, h, 2);
      ctx.fill();
    }

    // rodapé com o domínio atual do site
    ctx.font = '30px monospace';
    ctx.fillStyle = 'rgba(244,239,230,0.45)';
    ctx.fillText(window.location.hostname || 'falareal', 92, 980);
  }

  function updateShareVisibility(){
    if(streakData.streak > 0){
      shareBtn.style.display = 'block';
    }
  }

  shareBtn.addEventListener('click', ()=>{
    drawShareCard();
    sharePreview.style.display = sharePreview.style.display === 'none' ? 'block' : 'none';
  });

  downloadShareBtn.addEventListener('click', ()=>{
    drawShareCard();
    const link = document.createElement('a');
    link.download = 'falareal-sequencia.png';
    link.href = shareCanvas.toDataURL('image/png');
    link.click();
  });

  whatsappShareBtn.addEventListener('click', ()=>{
    const site = window.location.href;
    const text = currentLang === 'de'
      ? `🔥 ${streakData.streak} Tage in Folge echtes Deutsch geübt! ${site}`
      : `🔥 Bati ${streakData.streak} dias seguidos treinando alemão de verdade! ${site}`;
    window.open('https://wa.me/?text=' + encodeURIComponent(text), '_blank', 'noopener,noreferrer');
  });

  updateShareVisibility();

  // ---- Diagnóstico rápido (quiz) ----
  const quizAnswers = { desafio: null, nivel: null };

  const CHALLENGE_TEXT = {
    de: {
      sotaque: 'sotaques variados (níveis 3 e 4)',
      envolvimento: 'se envolver de verdade na vida daqui — comunidade, vizinhos, dia a dia',
      entrevista: 'cenários de entrevista de emprego',
      trabalho: 'conversas do dia a dia no trabalho'
    },
    en: {
      sotaque: 'varied accents (levels 3 and 4)',
      envolvimento: 'really getting involved in life here — community, neighbors, daily life',
      entrevista: 'job interview scenarios',
      trabalho: 'everyday work conversations'
    }
  };
  const LEVEL_BY_SELF = { '1':1, '2':2, '3':3 };

  function showQuizStep(step){
    document.querySelectorAll('.quiz-step').forEach(el=>{
      el.classList.toggle('active', el.getAttribute('data-step') === String(step));
    });
    document.querySelectorAll('.quiz-dot').forEach(el=>{
      const dot = el.getAttribute('data-dot');
      el.classList.toggle('active', dot === String(step));
      const order = ['1','2','result'];
      el.classList.toggle('done', order.indexOf(dot) < order.indexOf(String(step)));
    });
  }

  function finishQuiz(){
    const lang = currentLang;
    const desafioLabel = CHALLENGE_TEXT[lang][quizAnswers.desafio] || '';
    const level = LEVEL_BY_SELF[quizAnswers.nivel] || 2;

    document.getElementById('quiz-level-de').textContent = level;
    document.getElementById('quiz-level-en').textContent = level;
    document.getElementById('quiz-desc-de').textContent = `Baseado no que você respondeu, sugerimos focar em ${CHALLENGE_TEXT.de[quizAnswers.desafio] || 'cenários variados'}.`;
    document.getElementById('quiz-desc-en').textContent = `Based on your answers, we'd suggest focusing on ${CHALLENGE_TEXT.en[quizAnswers.desafio] || 'varied scenarios'}.`;

    // leva as respostas junto pro formulário de e-mail, e mostra um resuminho ali também
    const desafioBtnDe = document.querySelector(`.quiz-options.lang-de .quiz-option[data-key="${quizAnswers.desafio}"]`);
    const desafioBtnEn = document.querySelector(`.quiz-options.lang-en .quiz-option[data-key="${quizAnswers.desafio}"]`);
    document.getElementById('quiz-desafio-de').value = desafioBtnDe ? desafioBtnDe.dataset.label : '';
    document.getElementById('quiz-desafio-en').value = desafioBtnEn ? desafioBtnEn.dataset.label : '';
    document.getElementById('quiz-nivel-de').value = quizAnswers.nivel;
    document.getElementById('quiz-nivel-en').value = quizAnswers.nivel;

    const summaryDe = document.getElementById('quiz-summary-de');
    const summaryEn = document.getElementById('quiz-summary-en');
    summaryDe.textContent = `✓ Nível ${level} sugerido — foco em ${CHALLENGE_TEXT.de[quizAnswers.desafio] || 'cenários variados'}`;
    summaryEn.textContent = `✓ Level ${level} suggested — focus on ${CHALLENGE_TEXT.en[quizAnswers.desafio] || 'varied scenarios'}`;
    summaryDe.classList.add('show');
    summaryEn.classList.add('show');

    showQuizStep('result');
  }

  document.querySelectorAll('.quiz-step[data-step="1"] .quiz-option').forEach(btn=>{
    btn.addEventListener('click', ()=>{
      quizAnswers.desafio = btn.dataset.key;
      showQuizStep('2');
    });
  });
  document.querySelectorAll('.quiz-step[data-step="2"] .quiz-option').forEach(btn=>{
    btn.addEventListener('click', ()=>{
      quizAnswers.nivel = btn.dataset.key;
      finishQuiz();
    });
  });

  // ---- Sistema de indicação ----
  function getOrCreateMyCode(){
    try{
      let code = localStorage.getItem('falareal_ref_code');
      if(!code){
        code = Math.random().toString(36).slice(2, 8).toUpperCase();
        localStorage.setItem('falareal_ref_code', code);
      }
      return code;
    }catch(e){
      return Math.random().toString(36).slice(2, 8).toUpperCase();
    }
  }

  function getReferrerFromUrl(){
    const params = new URLSearchParams(window.location.search);
    return params.get('ref');
  }

  const myRefCode = getOrCreateMyCode();
  const referredBy = getReferrerFromUrl();
  if(referredBy){
    try{ localStorage.setItem('falareal_referred_by', referredBy); }catch(e){}
  }

  // guarda quem indicou (se veio de um link) nos campos ocultos dos formulários
  const storedReferrer = referredBy || (function(){ try{ return localStorage.getItem('falareal_referred_by'); }catch(e){ return null; } })();
  if(storedReferrer){
    const refDe = document.getElementById('ref-de');
    const refEn = document.getElementById('ref-en');
    if(refDe) refDe.value = storedReferrer;
    if(refEn) refEn.value = storedReferrer;
  }

  // monta o link pessoal de cada um, sem o parâmetro ref antigo (se houver)
  const baseUrl = window.location.origin + window.location.pathname;
  const myReferralLink = `${baseUrl}?ref=${myRefCode}`;

  const referralLinkDe = document.getElementById('referral-link-de');
  const referralLinkEn = document.getElementById('referral-link-en');
  if(referralLinkDe) referralLinkDe.value = myReferralLink;
  if(referralLinkEn) referralLinkEn.value = myReferralLink;

  function copyReferralLink(){
    navigator.clipboard.writeText(myReferralLink).catch(()=>{});
  }
  const copyDeBtn = document.getElementById('copy-referral-de');
  const copyEnBtn = document.getElementById('copy-referral-en');
  if(copyDeBtn) copyDeBtn.addEventListener('click', ()=>{
    copyReferralLink();
    copyDeBtn.textContent = '✓ Copiado';
    setTimeout(()=> copyDeBtn.textContent = '📋 Copiar', 1800);
  });
  if(copyEnBtn) copyEnBtn.addEventListener('click', ()=>{
    copyReferralLink();
    copyEnBtn.textContent = '✓ Copiado';
    setTimeout(()=> copyEnBtn.textContent = '📋 Copiar', 1800);
  });

  function shareReferralWhatsapp(lang){
    const text = lang === 'de'
      ? `Tô treinando alemão de verdade no Fala Real — sotaque, ruído, tudo real. Entra pelo meu link que a gente sobe junto na fila: ${myReferralLink}`
      : `I'm practicing real German/English on Fala Real — real accents, real noise. Join through my link so we move up the list together: ${myReferralLink}`;
    window.open('https://wa.me/?text=' + encodeURIComponent(text), '_blank', 'noopener,noreferrer');
  }
  const whatsappRefDe = document.getElementById('whatsapp-referral-de');
  const whatsappRefEn = document.getElementById('whatsapp-referral-en');
  if(whatsappRefDe) whatsappRefDe.addEventListener('click', ()=> shareReferralWhatsapp('de'));
  if(whatsappRefEn) whatsappRefEn.addEventListener('click', ()=> shareReferralWhatsapp('en'));

  // Waitlist forms — envia de verdade pro Formspree, mantendo a experiência inline
  const FORMSPREE_ENDPOINT = 'https://formspree.io/f/xeeywzdd';
  ['de','en'].forEach(lang=>{
    const form = document.getElementById('waitlist-form-' + lang);
    if(!form) return;
    form.addEventListener('submit', function(e){
      e.preventDefault();
      const emailInput = form.querySelector('input[type=email]');
      const submitBtn = form.querySelector('button[type=submit]');
      const originalBtnText = submitBtn.textContent;
      submitBtn.disabled = true;
      submitBtn.textContent = 'Enviando...';

      const formData = new FormData(form);
      formData.append('idioma', lang === 'de' ? 'alemão' : 'inglês');
      formData.append('origem', 'FalaReal landing page');

      fetch(FORMSPREE_ENDPOINT, {
        method: 'POST',
        headers: { 'Accept': 'application/json' },
        body: formData
      }).then(res=>{
        if(res.ok){
          document.getElementById('thanks-msg-' + lang).style.display = 'block';
          form.reset();
        } else {
          alert('Ops, algo deu errado. Tenta de novo em alguns segundos.');
        }
      }).catch(()=>{
        alert('Ops, algo deu errado. Tenta de novo em alguns segundos.');
      }).finally(()=>{
        submitBtn.disabled = false;
        submitBtn.textContent = originalBtnText;
      });
    });
  });
</script>

</body>
</html>
