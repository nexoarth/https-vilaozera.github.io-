# https-vilaozera.github.io-
Landing page oficial do VILÃOZERA — convite para lives, links para redes sociais e conteúdo de gameplay.
Copyright (c) 2025 [NEXOARTH]

Todos os direitos reservados.  

Este projeto é protegido por direitos autorais.  
Nenhuma parte deste site, incluindo HTML, CSS, JavaScript, textos e imagens,  
pode ser copiada, modificada, publicada ou distribuída sem permissão explícita do autor.
# Landing Page VILÃOZERA

Bem-vindo ao repositório da **Landing Page do VILÃOZERA**!  
Esta página foi criada para divulgar convites para lives, apresentar links das redes sociais e fornecer conteúdo de gameplay.

---

## 🎯 Objetivo

- Facilitar o compartilhamento do convite para a live do VILÃOZERA.
- Reunir links diretos para todas as redes sociais importantes.
- Oferecer uma interface simples e estilosa para os fãs interagirem.

---

## 🌐 Redes Sociais

A página contém links diretos para as principais redes sociais:

| Rede Social | Link |
|------------|------|
| YouTube | [https://m.youtube.com/@vilaozera](https://m.youtube.com/@vilaozera) |
| TikTok | [https://www.tiktok.com/@vilao_hs?_t=Z..](https://www.tiktok.com/@vilao_hs?_t=Z..) |
| Instagram (Ex Guilda FF) | [https://www.instagram.com/vlz_sport_ff](https://www.instagram.com/vlz_sport_ff) |
| Instagram Pessoal | [https://www.instagram.com/wesley_gabriel_vlz](https://www.instagram.com/wesley_gabriel_vlz) |
| Instagram Guilda | [https://www.instagram.com/head_shot_vlz](https://www.instagram.com/head_shot_vlz) |

---

## 💻 Tecnologias Utilizadas

- **HTML5** — estrutura da página
- **CSS3** — estilização e efeitos
- **JavaScript** — funcionalidades como copiar mensagem e redirecionamento no reload
- **Font Awesome** — ícones coloridos das redes sociais

---

## ⚡ Funcionalidades

- **Copiar mensagem** para enviar facilmente para o VILÃOZERA.
- **Botões de redes sociais** com ícones coloridos.
- **Cards de jogos** com efeitos visuais para interação.
- **Redirecionamento automático** para o YouTube caso a página seja atualizada.

---

## 📦 Como usar

1. Abra o arquivo `index.html` no navegador.
2. Clique nos botões para abrir redes sociais ou copiar a mensagem.
3. Para atualizar o site online, hospede no **GitHub Pages** ou outra plataforma de hospedagem gratuita.

---

## 🔗 Hospedagem Recomendada

- **GitHub Pages** — grátis e fácil de manter  
- **Netlify** — upload rápido via drag & drop  
- **Vercel** — simples para projetos estáticos

---

## ❤️ Contribuições

Este projeto é open source. Qualquer melhoria, correção ou sugestão é bem-vinda!  
Basta criar um pull request ou abrir uma issue.

---

Feito com ♥ por NEXOARTH 
<!doctype html>
<html lang="pt-BR">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Convite para live — VILÃOZERA</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
  <!-- Font Awesome para ícones oficiais -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2/css/all.min.css">

  <style>
    :root{
      --bg:#0f0f13;
      --card:#17171b;
      --accent:#ff4d4d;
      --muted:#bfbfc6;
      --glass: rgba(255,255,255,0.03);
      --radius:14px;
      font-family: Inter, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
    }
    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;
      background:linear-gradient(180deg,#09090b 0%, #0f0f13 60%);
      color:#fff;
      display:flex;
      align-items:center;
      justify-content:center;
      padding:24px;
      gap:20px;
    }

    .wrap{
      width:100%;
      max-width:980px;
      background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));
      border-radius:18px;
      padding:24px;
      box-shadow: 0 8px 30px rgba(0,0,0,0.6);
      display:grid;
      grid-template-columns: 1fr 360px;
      gap:20px;
      align-items:start;
    }

    .hero{padding:16px;border-radius:12px;background:linear-gradient(180deg, rgba(255,255,255,0.01), var(--glass));border:1px solid rgba(255,255,255,0.03);}
    h1{margin:0 0 8px 0;font-size:28px;letter-spacing:-0.5px;}
    p.lead{margin:0 0 16px 0;color:var(--muted);line-height:1.45;}
    .cta-row{display:flex; gap:12px; flex-wrap:wrap; margin-bottom:14px}
    .btn{
      display:inline-flex;align-items:center;gap:10px;
      padding:10px 14px;border-radius:10px;
      background:var(--accent);color:#fff;text-decoration:none;
      font-weight:600;border:none;cursor:pointer;
      box-shadow: 0 6px 18px rgba(255,77,77,0.12);
      transition:0.3s;
    }
    .btn:hover{transform:scale(1.05);}

    .channel-card{background:linear-gradient(180deg, rgba(255,255,255,0.01), rgba(255,255,255,0.02));border-radius:12px;padding:14px;text-align:center;border:1px solid rgba(255,255,255,0.03);}
    .avatar{width:92px;height:92px;border-radius:12px;background:linear-gradient(180deg,#2b2b2b,#111);display:inline-block;margin-bottom:10px;}
    .channel-name{font-weight:700;margin:6px 0 4px 0}
    .channel-sub{color:var(--muted);font-size:13px}
    .invite-box{margin-top:12px;background:rgba(0,0,0,0.25);border-radius:10px;padding:12px;font-family:ui-monospace,monospace;font-size:14px;color:#e9e9e9;line-height:1.35;}

    textarea{width:100%;min-height:118px;resize:vertical;background:transparent;color:inherit;border:1px dashed rgba(255,255,255,0.04);padding:12px;border-radius:8px;}

    .right{padding:12px;display:flex;flex-direction:column;gap:12px;}
    .small{font-size:13px;color:var(--muted);}
    .actions{display:flex;gap:10px;flex-wrap:wrap}
    footer{grid-column:1/-1;text-align:center;font-size:12px;color:var(--muted);margin-top:8px}

    .games-banner,.social-banner{display:flex;flex-direction:column;gap:12px;margin-top:16px;}
    .game-card,.social-card{
      background:var(--card);
      border:2px solid var(--accent);
      border-radius:12px;
      padding:12px;
      text-align:center;
      font-weight:600;
      font-size:14px;
      color:#fff;
      box-shadow: inset 0 0 10px rgba(255,77,77,0.5),0 0 15px var(--accent);
      transition:0.3s;
      cursor:pointer;
    }
    .game-card:hover,.social-card:hover{transform:scale(1.05);}
    .social-card i{margin-right:8px;font-size:18px;vertical-align:middle;}

    /* cores personalizadas */
    .youtube i{color:#ff0000;}
    .tiktok i{color:#00f2ea;}
    .instagram i{color:#e4405f;}

    .xp-bar{width:90%;height:6px;background:rgba(255,255,255,0.1);border-radius:4px;margin:6px auto 0;}
    .xp-fill{height:100%;background:linear-gradient(90deg,#ff0000,#ff4444);}
    @media(max-width:860px){.wrap{grid-template-columns:1fr;padding:16px}.right{order:2}}
  </style>
</head>
<body>
<main class="wrap">
  <section class="hero">
    <h1>Convite para live — VILÃOZERA</h1>
    <p class="lead">Use a mensagem pronta abaixo para convidar VILÃOZERA para suas lives, chats ou redes sociais.</p>
    <div class="cta-row">
      <a class="btn" href="https://youtube.com/@vilaozera" target="_blank">Abrir canal no YouTube</a>
    </div>
    <div class="invite-box">
      <textarea id="mensagem">Fala, VILÃOZERA! Quero muito acompanhar sua live e vibrar no chat. Tamo junto! — NEXOS</textarea>
      <div style="display:flex; gap:8px; margin-top:8px;">
        <button class="btn" id="copiar">Copiar mensagem</button>
      </div>
    </div>
  </section>

  <aside class="right">
    <div class="channel-card">
      <div class="avatar"></div>
      <div class="channel-name">VILÃOZERA</div>
      <div class="channel-sub">@vilaozera • canal de gameplay</div>
    </div>

    <!-- Redes sociais -->
    <div class="social-banner">
      <div class="small">Redes sociais</div>
      <a class="social-card youtube" href="https://m.youtube.com/@vilaozera" target="_blank"><i class="fab fa-youtube"></i>YouTube</a>
      <a class="social-card tiktok" href="https://www.tiktok.com/@vilao_hs?_t=Z.." target="_blank"><i class="fab fa-tiktok"></i>TikTok</a>
      <a class="social-card instagram" href="https://www.instagram.com/vlz_sport_ff" target="_blank"><i class="fab fa-instagram"></i>Instagram (Ex Guilda FF)</a>
      <a class="social-card instagram" href="https://www.instagram.com/wesley_gabriel_vlz" target="_blank"><i class="fab fa-instagram"></i>Instagram Pessoal</a>
      <a class="social-card instagram" href="https://www.instagram.com/head_shot_vlz" target="_blank"><i class="fab fa-instagram"></i>Instagram Guilda</a>
    </div>

    <!-- Jogos -->
    <div class="games-banner">
      <a class="game-card" href="#"><span>Minecraft</span><div class="xp-bar"><div class="xp-fill" style="width:80%"></div></div></a>
      <a class="game-card" href="#"><span>Repo</span><div class="xp-bar"><div class="xp-fill" style="width:60%"></div></div></a>
      <a class="game-card" href="#"><span>Blood Strike</span><div class="xp-bar"><div class="xp-fill" style="width:70%"></div></div></a>
      <a class="game-card" href="#"><span>Free Fire</span><div class="xp-bar"><div class="xp-fill" style="width:90%"></div></div></a>
      <a class="game-card" href="#"><span>Call of Duty Ops6</span><div class="xp-bar"><div class="xp-fill" style="width:75%"></div></div></a>
    </div>
  </aside>

  <footer>Feito com ♥ — personalize a mensagem e boa sorte com o convite!</footer>
</main>

<script>
  const copiarBtn = document.getElementById('copiar');
  const textarea = document.getElementById('mensagem');
  copiarBtn.addEventListener('click', async () => {
    try {
      await navigator.clipboard.writeText(textarea.value.trim());
      copiarBtn.textContent = 'Copiado!';
      setTimeout(()=> copiarBtn.textContent = 'Copiar mensagem', 2000);
    } catch (e){
      alert('Não foi possível copiar. Copie manualmente.');
    }
  });

  // Redireciona no reload
  const navEntries = performance.getEntriesByType("navigation");
  if (navEntries.length && navEntries[0].type === "reload") {
    window.location.href = "https://m.youtube.com/@vilaozera";
  }
</script>
</body>
</html>
