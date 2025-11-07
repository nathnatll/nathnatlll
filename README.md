<html lang="en">
<head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width,initial-scale=1" />
    <title>Nath Natll — Portfolio</title>
    <meta name="description" content="Minimalist portfolio for Nath Natll — projects, about, contact." />
    <style>
        :root{
            --bg:#0f1113;
            --card:#0b0c0d;
            --muted:#9aa2ad;
            --accent:#7dd3fc;
            --glass: rgba(255,255,255,0.03);
            --radius:12px;
            font-family: Inter, ui-sans-serif, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
        }
        *{box-sizing:border-box}
        html,body{height:100%}
        body{
            margin:0;
            background:
                radial-gradient(circle at 10% 10%, rgba(125,211,252,0.05), transparent 10%),
                linear-gradient(180deg,#050506 0%, var(--bg) 100%);
            color:#e6eef6;
            -webkit-font-smoothing:antialiased;
            -moz-osx-font-smoothing:grayscale;
            line-height:1.4;
            padding:48px 24px;
        }
        .wrap{max-width:980px;margin:0 auto}
        header{
            display:flex;
            align-items:center;
            justify-content:space-between;
            gap:16px;
            margin-bottom:36px;
        }
        .brand{
            display:flex;
            gap:16px;
            align-items:center;
        }
        .logo{
            width:56px;height:56px;border-radius:12px;
            background:linear-gradient(135deg,var(--accent),#89f7fe);
            display:grid;place-items:center;
            color:#031019;font-weight:700;font-size:18px;
            box-shadow:0 6px 18px rgba(12,17,23,0.6), inset 0 -6px 14px rgba(0,0,0,0.12);
        }
        h1{font-size:20px;margin:0}
        p.lead{margin:2px 0 0;color:var(--muted);font-size:13px}
        nav{display:flex;gap:12px;align-items:center}
        a.btn{
            color:var(--accent);text-decoration:none;font-weight:600;padding:10px 14px;border-radius:10px;
            background:linear-gradient(180deg, rgba(255,255,255,0.02), transparent);
            border:1px solid rgba(255,255,255,0.03);
            font-size:13px;
        }

        main{display:grid;grid-template-columns:1fr 320px;gap:28px;align-items:start}
        @media (max-width:860px){main{grid-template-columns:1fr;}}
        .hero{
            background:var(--glass);
            padding:28px;border-radius:var(--radius);
            border:1px solid rgba(255,255,255,0.03);
        }
        .intro h2{margin:0 0 8px;font-size:28px}
        .intro p{margin:0 0 18px;color:var(--muted)}
        .cta{display:flex;gap:10px;flex-wrap:wrap}
        .cta a{background:transparent;border:1px solid rgba(255,255,255,0.04);padding:10px 12px;border-radius:10px;text-decoration:none;color:var(--accent);font-weight:600}
        .projects{margin-top:18px;display:grid;grid-template-columns:repeat(2,1fr);gap:12px}
        @media (max-width:560px){.projects{grid-template-columns:1fr}}
        .card{
            background:linear-gradient(180deg, rgba(255,255,255,0.02), transparent);
            padding:12px;border-radius:10px;border:1px solid rgba(255,255,255,0.03);
            display:flex;flex-direction:column;gap:8px;
        }
        .thumb{
            height:110px;border-radius:8px;background:linear-gradient(135deg,#07101a,#0d1216);
            display:flex;align-items:center;justify-content:center;color:var(--muted);font-size:13px;border:1px dashed rgba(255,255,255,0.02);
        }
        .card h3{margin:0;font-size:15px}
        .card p{margin:0;color:var(--muted);font-size:13px}
        aside{
            position:relative;
        }
        .panel{
            background:linear-gradient(180deg, rgba(255,255,255,0.02), transparent);
            padding:18px;border-radius:var(--radius);border:1px solid rgba(255,255,255,0.03);
        }
        .about p{margin:0;color:var(--muted);font-size:14px}
        .links{display:flex;gap:10px;margin-top:12px;flex-wrap:wrap}
        .icon{
            display:inline-grid;place-items:center;width:38px;height:38px;border-radius:10px;
            background:rgba(255,255,255,0.02);color:var(--accent);text-decoration:none;border:1px solid rgba(255,255,255,0.03);
        }
        footer{margin-top:26px;color:var(--muted);font-size:13px;text-align:center}
        small{color:var(--muted)}
    </style>
</head>
<body>
    <div class="wrap">
        <header>
            <div class="brand">
                <div class="logo">NN</div>
                <div>
                    <h1>Nathaniel Bautista</h1>
                    <p class="lead">Designer & Frontend dev — Minimal, fast, accessible</p>
                </div>
            </div>
        </header>

        <main>
            <section class="hero" aria-labelledby="intro-title">
                <div class="intro">
                    <h2 id="intro-title">Hi — I build clean interfaces and simple portfolio.</h2>
                    <p>Focused on clarity, performance, and subtle interactions. I prefer small, maintainable projects that scale.</p>
                </div>

                <div class="cta" style="margin-top:12px">
                    <a href="#projects">Projects</a>
                    <a href="#contact">About me</a>
                </div>

                <div id="projects" class="projects" style="margin-top:18px">
                    <article class="card">
                        <div class="thumb">Project 1</div>
                        <h3>Coming soon</h3>
                    </article>

                </div>
            </section>
        </main>

        <footer>
            <small>© <span id="year"></span> Nath Natll — Built with HTML & CSS</small>
        </footer>
    </div>

    <script>
        // Small niceties
        document.getElementById('year').textContent = new Date().getFullYear();
    </script>
</body>
</html>
