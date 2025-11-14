<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Gym Management System — README Preview</title>
  <style>
    :root{
      --bg:#0f1724; --card:#0b1220; --muted:#94a3b8; --accent1:#06b6d4; --accent2:#7c3aed; --glass: rgba(255,255,255,0.04);
      --radius:14px; --maxw:1000px;
      font-family: Inter, ui-sans-serif, system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial;
    }
    *{box-sizing:border-box}
    body{background:linear-gradient(180deg,var(--bg),#041027); color:#e6eef8; margin:0; -webkit-font-smoothing:antialiased}
    .wrap{max-width:var(--maxw); margin:40px auto; padding:28px}

    .hero{display:grid;grid-template-columns:1fr 360px;gap:28px;align-items:center}
    .logo{display:flex;gap:12px;align-items:center}
    .badge{background:linear-gradient(90deg,var(--accent1),var(--accent2)); padding:10px;border-radius:12px; box-shadow:0 6px 20px rgba(124,58,237,0.18)}
    .badge svg{display:block}
    h1{margin:0 0 6px 0;font-size:28px}
    p.lead{margin:0;color:var(--muted)}

    .card{background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01)); padding:18px;border-radius:var(--radius);box-shadow: 0 6px 30px rgba(2,6,23,0.6);}

    .grid{display:grid; grid-template-columns:repeat(2,1fr); gap:14px; margin-top:18px}
    .feature{padding:14px;border-radius:12px;background:var(--glass);}
    .feature h3{margin:0 0 6px 0;font-size:15px}
    .meta{font-size:13px;color:var(--muted)}

    .screenshot{height:160px;border-radius:10px;background:linear-gradient(135deg, rgba(255,255,255,0.03), rgba(255,255,255,0.01));display:flex;align-items:center;justify-content:center;color:var(--muted);font-size:13px}

    .badges{display:flex;gap:8px;flex-wrap:wrap;margin-top:14px}

    pre{background:#071028;padding:16px;border-radius:10px;overflow:auto;color:#cce7ff}

    .actions{display:flex;gap:8px; margin-top:12px}
    .btn{padding:10px 14px;border-radius:10px;background:linear-gradient(90deg,var(--accent1),var(--accent2));border:none;color:#061021;font-weight:600;cursor:pointer;text-decoration:none}
    .btn.ghost{background:transparent;color:var(--accent1);border:1px solid rgba(255,255,255,0.04)}

    footer{margin-top:20px;color:var(--muted);font-size:13px;text-align:center}

    @media (max-width:900px){.hero{grid-template-columns:1fr;}.grid{grid-template-columns:1fr}}
  </style>
</head>
<body>
  <div class="wrap">
    <div class="hero">
      <div>
        <div class="card">
          <div class="logo">
            <div class="badge" aria-hidden>
              <!-- dumbbell SVG -->
              <svg width="36" height="36" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M2 8h2v8H2zM20 8h2v8h-2zM7 7h10v10H7z" fill="white" opacity="0.97"/>
              </svg>
            </div>
            <div>
              <h1>Gym Management System</h1>
              <p class="lead">Clean, lightweight web interface for managing members, attendance, subscriptions and payments.</p>
            </div>
          </div>

          <div class="badges" role="img" aria-label="badges">
            <img src="https://img.shields.io/badge/Status-Production-green" alt="status" />
            <img src="https://img.shields.io/badge/Stack-Flask%20%7C%20SQLite-blue" alt="stack" />
            <img src="https://img.shields.io/badge/License-MIT-yellow" alt="license" />
          </div>

          <div class="grid">
            <div class="feature">
              <h3>✨ Key features</h3>
              <div class="meta">Member profiles, plans & billing, check-in/out, reports, CSV export, user roles.</div>
            </div>
            <div class="feature">
              <h3>🔒 Auth & roles</h3>
              <div class="meta">Admin, Trainer and Receptionist roles with password hashing and session management.</div>
            </div>
            <div class="feature">
              <h3>📊 Reports</h3>
              <div class="meta">Attendance charts, revenue summaries, and monthly export for pricing & audits.</div>
            </div>
            <div class="feature">
              <h3>⚡ Quick start</h3>
              <div class="meta">Clone, create virtualenv, install requirements, run `flask run`.</div>
            </div>
          </div>

          <div class="actions">
            <a class="btn" href="#installation">Get started</a>
            <a class="btn ghost" href="#demo">Live demo</a>
          </div>
        </div>
      </div>

      <aside>
        <div class="card">
          <div class="screenshot">Screenshot / GIF placeholder</div>
          <div style="margin-top:12px">
            <strong>Tech stack</strong>
            <div class="meta">Flask • SQLite / PostgreSQL • Bootstrap/Tailwind • JS (optional)</div>
          </div>
        </div>
      </aside>
    </div>

    <section style="margin-top:18px">
      <div class="card">
        <h2 style="margin-top:0">Installation</h2>
        <pre><code>git clone https://github.com/youruser/gym-management.git
cd gym-management
python -m venv .venv
source .venv/bin/activate   # or .venv\Scripts\activate on Windows
pip install -r requirements.txt
export FLASK_APP=app.py
flask run
</code></pre>

        <h2 id="demo">Usage & Tips</h2>
        <ul class="meta">
          <li>Create an admin user with `flask create-admin`.</li>
          <li>Import members by CSV via Admin → Import.</li>
          <li>Enable daily backups for the DB file in production.</li>
        </ul>

        <h2 id="contribute">Contributing</h2>
        <div class="meta">PRs welcome — follow the code style, add tests for new features, and keep migrations small.</div>

        <h2 id="license">License</h2>
        <div class="meta">MIT © Your Name</div>

        <h2 id="snippets">Example README snippet (Markdown)</h2>
        <pre><code>## Gym Management System

A lightweight gym management web application built with Flask.

**Features**: Member management, attendance, plans, billing, reports.

**Quick start**:
```bash
git clone ...
```</code></pre>
      </div>
    </section>

    <footer>
      Built with ❤️ — copy this HTML into your `README.md` (GitHub supports many HTML elements) or host `readme_preview.html` to share a live snapshot.
    </footer>
  </div>
</body>
</html>
