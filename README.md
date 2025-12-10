<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>My First GitLab Pages — Welcome!</title>
  <meta name="description" content="My first GitLab Pages site — simple, responsive landing page." />

  <style>
    :root{
      --bg:#0f1724;
      --card:#0b1220;
      --accent:#7dd3fc;
      --muted:#9aa4b2;
      --glass: rgba(255,255,255,0.03);
      --radius:12px;
      font-family: Inter, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
    }
    *{box-sizing:border-box}
    html,body{height:100%;}
    body{
      margin:0;
      background: linear-gradient(180deg, #071026 0%, #021223 100%);
      color: #e6eef6;
      -webkit-font-smoothing:antialiased;
      line-height:1.5;
      display:flex;
      align-items:center;
      justify-content:center;
      padding:32px;
    }

    .wrap{
      width:100%;
      max-width:980px;
      background: linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));
      border-radius:18px;
      padding:28px;
      box-shadow: 0 8px 30px rgba(2,6,23,0.6);
      border: 1px solid rgba(255,255,255,0.03);
    }

    header{
      display:flex;
      align-items:center;
      justify-content:space-between;
      gap:16px;
      margin-bottom:18px;
    }

    .brand{
      display:flex;
      gap:12px;
      align-items:center;
    }

    .logo{
      width:56px;
      height:56px;
      border-radius:12px;
      background:linear-gradient(135deg,var(--accent), #60a5fa);
      display:flex;
      align-items:center;
      justify-content:center;
      color:#012233;
      font-weight:700;
      font-size:20px;
      box-shadow: 0 6px 18px rgba(125,211,252,0.08);
    }

    h1{
      margin:0;
      font-size:20px;
      letter-spacing:-0.2px;
    }

    p.lead {
      margin:6px 0 0;
      color:var(--muted);
      font-size:14px;
    }

    .actions{
      display:flex;
      gap:8px;
    }

    .btn {
      background:transparent;
      color:var(--accent);
      border:1px solid rgba(125,211,252,0.18);
      padding:8px 12px;
      border-radius:10px;
      font-weight:600;
      text-decoration:none;
      transition:all 160ms ease;
    }
    .btn.primary{
      background:linear-gradient(90deg,var(--accent),#60a5fa);
      color:#032034;
      border: none;
      box-shadow: 0 6px 18px rgba(96,165,250,0.08);
    }
    .btn:hover{transform:translateY(-2px)}

    main{
      display:grid;
      grid-template-columns:1fr 320px;
      gap:18px;
      margin-top:12px;
    }

    .hero {
      background:var(--glass);
      padding:18px;
      border-radius:12px;
      min-height:220px;
    }

    h2{margin-top:0}
    ul.features{
      padding-left:18px;
      color:var(--muted);
      margin-top:10px;
    }

    .card {
      background: linear-gradient(180deg, rgba(255,255,255,0.01), rgba(255,255,255,0.00));
      border-radius:12px;
      padding:14px;
      border:1px solid rgba(255,255,255,0.02);
    }

    .sidebar .meta {
      display:flex;
      gap:8px;
      align-items:center;
      margin-bottom:12px;
    }

    code.inline {
      background: rgba(0,0,0,0.28);
      padding:4px 8px;
      border-radius:6px;
      font-family: ui-monospace, SFMono-Regular, Menlo, Monaco, "Roboto Mono", monospace;
      font-size:13px;
      color:#dff6ff;
    }

    footer{
      margin-top:16px;
      color:var(--muted);
      font-size:13px;
      display:flex;
      justify-content:space-between;
      align-items:center;
      gap:12px;
      flex-wrap:wrap;
    }

    @media (max-width:880px){
      main{grid-template-columns:1fr}
      .logo{width:48px;height:48px;font-size:18px}
    }
  </style>
</head>
<body>
  <div class="wrap" role="main">
    <header>
      <div class="brand" aria-hidden="false">
        <div class="logo">GL</div>
        <div>
          <h1>My First GitLab Pages</h1>
          <p class="lead">A minimal site deployed from GitLab — built for learning and showcasing projects.</p>
        </div>
      </div>

      <div class="actions" aria-hidden="false">
        <a class="btn" href="#how-to">How to deploy</a>
        <a class="btn primary" href="https://gitlab.com" target="_blank" rel="noopener">Open GitLab</a>
      </div>
    </header>

    <main>
      <section class="hero card" aria-label="Site introduction">
        <h2>Welcome 👋</h2>
        <p style="color:var(--muted)">This is a simple static landing page you can use as a starting point for your GitLab Pages site. Edit <code class="inline">index.html</code>, push to your repository, and the pipeline will publish your site.</p>

        <h3 style="margin-top:12px">What you get</h3>
        <ul class="features">
          <li>Responsive single-file HTML + CSS (no build tools required)</li>
          <li>One-click deploy with the provided <code class="inline">.gitlab-ci.yml</code></li>
          <li>Easy to customize — change text, colors, or add images</li>
        </ul>

        <h3 style="margin-top:12px">Customize</h3>
        <p class="lead" style="color:var(--muted)">Open this file, change the content, replace the logo, or add sections. For advanced projects you can add assets in a <code class="inline">public/</code> directory and update the pipeline accordingly.</p>
      </section>

      <aside class="sidebar">
        <div class="card">
          <div class="meta">
            <strong>Project</strong>
            <span style="margin-left:auto;color:var(--muted)">Static • HTML</span>
          </div>

          <p style="color:var(--muted);margin-top:0">Quick commands (locally):</p>
          <pre style="background:rgba(0,0,0,0.18);padding:10px;border-radius:8px;color:#e6eef6;font-size:13px;margin:10px 0">
# serve locally (node http-server)
npx http-server -c-1

