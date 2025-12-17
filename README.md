# Proyecto-final-

<!doctype html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>AWS - Página Demo</title>
  <style>
    :root{
      --bg:#0b1220;
      --card:#111a2e;
      --text:#e9eefc;
      --muted:#b7c3e6;
      --accent:#ff9900;
      --line:rgba(255,255,255,.12);
    }
    *{box-sizing:border-box}
    body{
      margin:0;
      font-family:system-ui,-apple-system,Segoe UI,Roboto,Arial,sans-serif;
      background:linear-gradient(180deg,#070b14 0%, #0b1220 60%, #060812 100%);
      color:var(--text);
    }
    a{color:inherit;text-decoration:none}
    .wrap{max-width:1100px;margin:0 auto;padding:0 18px}
    header{
      position:sticky; top:0; z-index:10;
      backdrop-filter:blur(10px);
      background:rgba(6,8,18,.65);
      border-bottom:1px solid var(--line);
    }
    nav{
      display:flex; align-items:center; justify-content:space-between;
      padding:14px 0;
      gap:14px;
    }
    .brand{
      display:flex; align-items:center; gap:10px; font-weight:800; letter-spacing:.2px;
    }
    .logo{
      width:34px;height:34px;border-radius:10px;
      background:radial-gradient(circle at 30% 30%, #ffd28a 0%, #ff9900 40%, #c46b00 100%);
      box-shadow:0 10px 30px rgba(255,153,0,.25);
    }
    .links{display:flex; gap:14px; flex-wrap:wrap}
    .links a{
      padding:8px 10px;border-radius:10px;color:var(--muted);
    }
    .links a:hover{background:rgba(255,255,255,.06); color:var(--text)}
    .btn{
      display:inline-flex; align-items:center; justify-content:center;
      padding:10px 14px; border-radius:12px; font-weight:700;
      border:1px solid var(--line); background:rgba(255,255,255,.06);
    }
    .btn.primary{
      background:var(--accent); color:#1a1205; border-color:transparent;
      box-shadow:0 14px 35px rgba(255,153,0,.25);
    }
    .btn.primary:hover{filter:brightness(1.05)}
    .hero{
      padding:54px 0 26px;
    }
    .hero-grid{
      display:grid; grid-template-columns:1.2fr .8fr; gap:22px; align-items:stretch;
    }
    .headline{
      font-size:clamp(28px,4vw,46px);
      line-height:1.05; margin:0 0 12px;
    }
    .sub{
      margin:0 0 18px; color:var(--muted); font-size:clamp(14px,1.5vw,18px);
    }
    .pill-row{display:flex; gap:10px; flex-wrap:wrap; margin:16px 0 20px}
    .pill{
      border:1px solid var(--line);
      background:rgba(255,255,255,.04);
      padding:8px 10px; border-radius:999px; color:var(--muted); font-size:13px;
    }
    .card{
      background:linear-gradient(180deg, rgba(255,255,255,.06), rgba(255,255,255,.03));
      border:1px solid var(--line);
      border-radius:18px;
      padding:18px;
    }
    .stat{
      display:grid; gap:10px;
    }
    .stat h3{margin:0; font-size:16px}
    .stat p{margin:0; color:var(--muted); font-size:13px}
    .grid{
      display:grid; gap:14px;
      grid-template-columns:repeat(3, minmax(0,1fr));
    }
    section{padding:26px 0}
    h2{margin:0 0 12px; font-size:22px}
    .muted{color:var(--muted)}
    .service{
      padding:16px;
      border-radius:16px;
      border:1px solid var(--line);
      background:rgba(17,26,46,.6);
    }
    .service b{display:block; margin-bottom:6px}
    .service small{color:var(--muted); line-height:1.4}
    .cta{
      display:flex; align-items:center; justify-content:space-between;
      gap:14px; flex-wrap:wrap;
    }
    footer{
      padding:22px 0 40px;
      border-top:1px solid var(--line);
      color:var(--muted);
      font-size:13px;
    }
    @media (max-width: 900px){
      .hero-grid{grid-template-columns:1fr}
      .grid{grid-template-columns:1fr}
    }
  </style>
</head>

<body>
  <header>
    <div class="wrap">
      <nav>
        <div class="brand">
          <div class="logo" aria-hidden="true"></div>
          <span>AWS • Demo</span>
        </div>
        <div class="links">
          <a href="#que-es">¿Qué es?</a>
          <a href="#servicios">Servicios</a>
          <a href="#beneficios">Beneficios</a>
          <a href="#empezar">Empezar</a>
        </div>
        <a class="btn primary" href="#empezar">Crear cuenta</a>
      </nav>
    </div>
  </header>

  <main class="wrap">
    <section class="hero" id="top">
      <div class="hero-grid">
        <div class="card">
          <h1 class="headline">Amazon Web Services (AWS)</h1>
          <p class="sub">
            Una página de ejemplo en HTML para presentar AWS: nube, cómputo, almacenamiento,
            bases de datos y más. (Contenido informativo, no oficial).
          </p>

          <div class="pill-row">
            <span class="pill">Escalable</span>
            <span class="pill">Pago por uso</span>
            <span class="pill">Alta disponibilidad</span>
            <span class="pill">Seguridad</span>
          </div>

          <div style="display:flex; gap:10px; flex-wrap:wrap;">
            <a class="btn primary" href="#servicios">Ver servicios</a>
            <a class="btn" href="#beneficios">¿Por qué AWS?</a>
          </div>
        </div>

        <div class="card stat" aria-label="Resumen">
          <h3>Resumen rápido</h3>
          <p>• Nube pública con muchos servicios.</p>
          <p>• Infraestructura global (regiones y zonas).</p>
          <p>• Ideal para apps web, APIs, datos y ML.</p>
          <hr style="border:none;border-top:1px solid var(--line);margin:8px 0">
          <h3>Ejemplos de uso</h3>
          <p>Hosting, backups, bases de datos, contenedores, serverless.</p>
        </div>
      </div>
    </section>

    <section id="que-es">
      <h2>¿Qué es AWS?</h2>
      <p class="muted">
        AWS es una plataforma de servicios en la nube que permite crear y desplegar aplicaciones
        sin comprar servidores físicos. Tú eliges los servicios que necesitas y pagas por lo que usas.
      </p>
    </section>

    <section id="servicios">
      <h2>Servicios populares</h2>
      <div class="grid">
        <div class="service">
          <b>EC2 (Compute)</b>
          <small>Máquinas virtuales para ejecutar aplicaciones con control total del servidor.</small>
        </div>
        <div class="service">
          <b>S3 (Storage)</b>
          <small>Almacenamiento de objetos para archivos, backups, imágenes y contenido estático.</small>
        </div>
        <div class="service">
          <b>RDS (Database)</b>
          <small>Bases de datos administradas (MySQL, PostgreSQL, etc.) con mantenimiento simplificado.</small>
        </div>
        <div class="service">
          <b>Lambda (Serverless)</b>
          <small>Ejecuta código por eventos sin administrar servidores. Pagas por ejecución.</small>
        </div>
        <div class="service">
          <b>CloudFront (CDN)</b>
          <small>Entrega contenido rápido con caché global para mejorar rendimiento.</small>
        </div>
        <div class="service">
          <b>IAM (Security)</b>
          <small>Control de accesos, usuarios, roles y permisos dentro de tu cuenta.</small>
        </div>
      </div>
    </section>

    <section id="beneficios">
      <h2>Beneficios</h2>
      <div class="grid">
        <div class="card">
          <b>Escalabilidad</b>
          <p class="muted">Sube o baja recursos según demanda sin comprar hardware.</p>
        </div>
        <div class="card">
          <b>Confiabilidad</b>
          <p class="muted">Diseñado para alta disponibilidad con opciones multi-zona.</p>
        </div>
        <div class="card">
          <b>Seguridad</b>
          <p class="muted">Herramientas para cifrado, control de acceso y auditoría.</p>
        </div>
      </div>
    </section>

    <section id="empezar">
      <div class="card cta">
        <div>
          <h2 style="margin:0 0 6px">¿Listo para empezar?</h2>
          <div class="muted">Crea un proyecto demo y prueba servicios como S3 o EC2.</div>
        </div>
        <div style="display:flex; gap:10px; flex-wrap:wrap;">
          <button class="btn primary" onclick="alert('Demo: aquí podrías enlazar al registro de AWS.')">
            Crear cuenta (demo)
          </button>
          <button class="btn" onclick="document.getElementById('top').scrollIntoView({behavior:'smooth'})">
            Volver arriba
          </button>
        </div>
      </div>
    </section>

    <footer>
      <div class="wrap">
        <div>© 2025 • Página demo hecha en HTML + CSS • No afiliada a Amazon.</div>
      </div>
    </footer>
  </main>
<div id="resultado"></div>

<script>
async function cargarInfo() {
  const url = "https://mnwbsk713a.execute-api.us-east-1.amazonaws.com/prod/info";
  const res = await fetch(url);
  const data = await res.json();

  document.getElementById("resultado").innerHTML =
    `<h3>${data.mensaje}</h3><p>${data.fecha_hora}</p>`;
}

cargarInfo();
</script>

</body>
</html>
