<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Python Basics</title>
  <style>
    :root{
      --bg:#f6fbff;
      --card:#ffffff;
      --accent:#0b63d9;
      --text:#0f1723;
      --muted:#556074;
      --radius:12px;
      --shadow: 0 6px 18px rgba(12, 40, 80, 0.08);
      font-family: Inter, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
    }
    body{
      margin:0;
      min-height:100vh;
      display:flex;
      align-items:center;
      justify-content:center;
      background:linear-gradient(180deg,var(--bg),#eef6ff);
      color:var(--text);
      padding:32px;
    }
    .card{
      max-width:720px;
      background:var(--card);
      border-radius:var(--radius);
      box-shadow:var(--shadow);
      padding:28px;
      border:1px solid rgba(11,99,217,0.06);
    }
    .kicker{
      display:inline-block;
      background:rgba(11,99,217,0.08);
      color:var(--accent);
      font-weight:600;
      padding:6px 10px;
      border-radius:8px;
      font-size:13px;
      margin-bottom:12px;
    }
    h1{
      margin:4px 0 12px;
      font-size:20px;
      letter-spacing:-0.2px;
    }
    p{
      margin:0;
      line-height:1.65;
      color:var(--muted);
      font-size:15px;
    }
    @media (prefers-color-scheme: dark) {
      :root{
        --bg:#071025;
        --card:#071428;
        --accent:#58a6ff;
        --text:#e6eef8;
        --muted:#a9bbd6;
        --shadow: 0 8px 24px rgba(2,6,23,0.6);
      }
    }
  </style>
</head>
<body>
  <article class="card" role="article" aria-labelledby="title">
    <div class="kicker">Programming</div>
    <h1 id="title">Python basics</h1>
    <p>
      Python is a high-level, interpreted programming language known for clear, readable syntax and a large standard library that speeds development. It supports multiple programming paradigms — procedural, object-oriented, and functional — making it suitable for beginners and experienced developers alike. Common uses include web development, data analysis, scripting, automation, and scientific computing. Python's package ecosystem (installed via pip) provides libraries for almost any task, and its interactive REPL and simple file-based scripts make it easy to experiment and iterate quickly.
    </p>
  </article>
</body>
</html>