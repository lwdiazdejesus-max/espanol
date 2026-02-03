[<!doctype html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Español 9 y 10 | Escuela José Collazo Colón</title>
  <meta name="description" content="Página de clase: Lectura, Gramática y Ortografía. Español 9 y 10." />

  <style>
    :root{
      --bg:#0b1020;
      --card:#111a33;
      --text:#eef2ff;
      --muted:#c7d2fe;
      --accent:#ffd166;
      --accent2:#80ffdb;
      --line:rgba(255,255,255,.14);
      --shadow: 0 18px 40px rgba(0,0,0,.35);
      --radius: 18px;
    }
    *{box-sizing:border-box}
    body{
      margin:0;
      font-family: system-ui, -apple-system, Segoe UI, Roboto, Arial, sans-serif;
      color:var(--text);
      background: radial-gradient(900px 500px at 20% 10%, rgba(128,255,219,.15), transparent 60%),
                  radial-gradient(800px 500px at 80% 10%, rgba(255,209,102,.18), transparent 55%),
                  linear-gradient(180deg, var(--bg), #060913 70%);
      line-height:1.5;
    }
    a{color:inherit}
    .wrap{max-width:1100px; margin:0 auto; padding:22px}
    header{
      position:sticky; top:0; z-index:10;
      backdrop-filter: blur(10px);
      background: rgba(6,9,19,.75);
      border-bottom:1px solid var(--line);
    }
    .topbar{display:flex; gap:16px; align-items:center; justify-content:space-between; padding:14px 22px}
    .brand{display:flex; gap:12px; align-items:center}
    .logo{
      width:42px; height:42px; border-radius:14px;
      background: linear-gradient(135deg, var(--accent), var(--accent2));
      box-shadow: var(--shadow);
    }
    .brand h1{font-size:16px; margin:0}
    .brand p{margin:0; font-size:12px; color:var(--muted)}
    nav{display:flex; gap:10px; flex-wrap:wrap}
    nav a{
      text-decoration:none;
      font-size:13px;
      padding:9px 12px;
      border:1px solid var(--line);
      border-radius:999px;
      background: rgba(255,255,255,.04);
    }
    nav a:hover{border-color: rgba(255,255,255,.35)}

    .hero{
      padding:26px 0 12px;
      display:grid;
      grid-template-columns: 1.15fr .85fr;
      gap:18px;
      align-items:stretch;
    }
    @media (max-width: 900px){
      .hero{grid-template-columns: 1fr}
    }
    .panel{
      background: rgba(255,255,255,.04);
      border:1px solid var(--line);
      border-radius: var(--radius);
      box-shadow: var(--shadow);
      overflow:hidden;
    }
    .panel .pad{padding:18px}
    .kicker{color:var(--muted); font-size:13px; margin:0 0 6px}
    .title{font-size:28px; margin:0 0 10px; letter-spacing:.2px}
    .subtitle{margin:0 0 14px; color:rgba(255,255,255,.86)}
    .chips{display:flex; flex-wrap:wrap; gap:10px; margin-top:12px}
    .chip{
      font-size:12px;
      padding:8px 10px;
      border-radius:999px;
      border:1px solid var(--line);
      background: rgba(255,255,255,.03);
      color: rgba(255,255,255,.92);
    }
    .ctaRow{display:flex; gap:10px; flex-wrap:wrap; margin-top:14px}
    .btn{
      display:inline-block;
      text-decoration:none;
      font-weight:600;
      font-size:13px;
      padding:10px 14px;
      border-radius: 12px;
      border:1px solid var(--line);
      background: rgba(255,255,255,.05);
    }
    .btn.primary{
      background: linear-gradient(135deg, rgba(255,209,102,.95), rgba(128,255,219,.85));
      color:#0b1020;
      border-color: transparent;
    }
    .btn:hover{transform: translateY(-1px)}
    .heroImg{
      display:grid;
      grid-template-rows: 1fr 1fr;
      gap:12px;
      padding:12px;
    }
    .imgCard{
      position:relative;
      border-radius: 16px;
      overflow:hidden;
      border:1px solid var(--line);
      min-height: 160px;
      background:#0b1020;
    }
    .imgCard img{
      width:100%; height:100%;
      object-fit:cover;
      display:block;
      filter: saturate(1.05) contrast(1.03);
      opacity:.92;
    }
    .imgTag{
      position:absolute; left:12px; bottom:12px;
      font-size:12px;
      padding:7px 10px;
      border-radius:999px;
      background: rgba(0,0,0,.45);
      border:1px solid rgba(255,255,255,.18);
    }

    main{padding:10px 0 30px}
    .grid{
      display:grid;
      grid-template-columns: 1fr 1fr;
      gap:18px;
      margin-top:18px;
    }
    @media (max-width: 900px){
      .grid{grid-template-columns: 1fr}
    }
    section{scroll-margin-top:90px}
    .sectionHead{
      display:flex; align-items:flex-end; justify-content:space-between; gap:12px;
      margin:0 0 10px;
    }
    .sectionHead h2{margin:0; font-size:18px}
    .sectionHead .hint{margin:0; font-size:13px; color:var(--muted)}
    .card{
      background: rgba(255,255,255,.04);
      border:1px solid var(--line);
      border-radius: var(--radius);
      box-shadow: var(--shadow);
      overflow:hidden;
    }
    .card .pad{padding:16px}
    .list{
      margin:10px 0 0; padding:0; list-style:none;
      display:grid; gap:10px;
    }
    .item{
      border:1px solid var(--line);
      border-radius:14px;
      padding:12px;
      background: rgba(255,255,255,.03);
    }
    .item h3{margin:0 0 6px; font-size:15px}
    .item p{margin:0; color: rgba(255,255,255,.86); font-size:13px}
    .meta{margin-top:8px; display:flex; gap:8px; flex-wrap:wrap}
    .tag{
      font-size:12px; color: rgba(255,255,255,.9);
      border:1px solid var(--line);
      background: rgba(255,255,255,.02);
      padding:6px 8px; border-radius:999px;
    }

    details{
      border:1px solid var(--line);
      border-radius: 14px;
      padding:12px;
      background: rgba(255,255,255,.03);
    }
    details + details{margin-top:10px}
    summary{cursor:pointer; font-weight:700}
    summary span{font-weight:500; color:var(--muted)}
    .twoCol{
      display:grid; gap:12px;
      grid-template-columns: 1fr 1fr;
      margin-top:12px;
    }
    @media (max-width: 700px){
      .twoCol{grid-template-columns: 1fr}
    }
    .mini{
      border:1px dashed rgba(255,255,255,.20);
      border-radius: 14px;
      padding:12px;
      background: rgba(255,255,255,.02);
    }
    .mini h4{margin:0 0 6px; font-size:14px}
    .mini ul{margin:0; padding-left:18px}
    .mini li{margin:6px 0; color: rgba(255,255,255,.88); font-size:13px}

    .footer{
      margin-top:22px;
      padding:18px;
      border-top:1px solid var(--line);
      color:rgba(255,255,255,.78);
      font-size:12px;
    }
    .note{
      font-size:12px;
      color: var(--muted);
      margin-top:10px;
    }
    .search{
      display:flex; gap:10px; flex-wrap:wrap; align-items:center;
      margin-top:12px;
    }
    input[type="search"]{
      flex:1;
      min-width: 220px;
      padding:10px 12px;
      border-radius: 12px;
      border:1px solid var(--line);
      background: rgba(255,255,255,.03);
      color:var(--text);
      outline:none;
    }
    .smallBtn{
      padding:10px 12px;
      border-radius: 12px;
      border:1px solid var(--line);
      background: rgba(255,255,255,.05);
      color:var(--text);
      cursor:pointer;
      font-weight:600;
    }
  </style>
</head>

<body>
  <header>
    <div class="topbar">
      <div class="brand">
        <div class="logo" aria-hidden="true"></div>
        <div>
          <h1>Español 9 y 10</h1>
          <p>Escuela José Collazo Colón · Puerto Rico</p>
        </div>
      </div>
      <nav aria-label="Navegación principal">
        <a href="#inicio">Inicio</a>
        <a href="#lectura">Lectura</a>
        <a href="#gramatica">Gramática</a>
        <a href="#ortografia">Ortografía</a>
        <a href="#recursos">Recursos</a>
      </nav>
    </div>
  </header>

  <div class="wrap" id="inicio">
    <div class="hero">
      <div class="panel">
        <div class="pad">
          <p class="kicker">Bienvenidos/as</p>
          <h2 class="title">Tu espacio de clase: Lectura · Gramática · Ortografía</h2>
          <p class="subtitle">
            Aquí encontrarás lecturas, actividades y recordatorios. Esta página está diseñada para estudiantes de
            <strong>Español 9 y 10</strong>.
          </p>

          <div class="chips" aria-label="Temas principales">
            <div class="chip">Comprensión lectora</div>
            <div class="chip">Análisis de texto</div>
            <div class="chip">Gramática y sintaxis</div>
            <div class="chip">Acentuación</div>
            <div class="chip">Redacción</div>
          </div>

          <div class="ctaRow">
            <a class="btn primary" href="#lectura">Ir a Lectura</a>
            <a class="btn" href="#gramatica">Ir a Gramática</a>
            <a class="btn" href="#ortografia">Ir a Ortografía</a>
          </div>

          <div class="search" aria-label="Búsqueda rápida">
            <input id="buscador" type="search" placeholder="Buscar: 'acentuación', 'cuento', 'sintaxis'..." />
            <button class="smallBtn" onclick="buscar()">Buscar</button>
            <button class="smallBtn" onclick="limpiar()">Limpiar</button>
          </div>
          <p class="note">Tip: Escribe una palabra y presiona “Buscar” para resaltar coincidencias.</p>
        </div>
      </div>

      <div class="panel heroImg" aria-label="Imágenes de cultura puertorriqueña">
        <!-- Imágenes desde Wikimedia Commons (gratuitas). Puedes cambiarlas por otras si deseas. -->
        <div class="imgCard">
          <img src="https://upload.wikimedia.org/wikipedia/commons/4/49/Old_San_Juan%2C_Puerto_Rico.jpg" alt="Calle en el Viejo San Juan, Puerto Rico" />
          <div class="imgTag">Viejo San Juan</div>
        </div>
        <div class="imgCard">
          <img src="https://upload.wikimedia.org/wikipedia/commons/4/4a/Castillo_San_Felipe_del_Morro%2C_San_Juan%2C_Puerto_Rico.jpg" alt="Castillo San Felipe del Morro, San Juan" />
          <div class="imgTag">El Morro</div>
        </div>
      </div>
    </div>

    <main>
      <div class="grid">
        <!-- LECTURA -->
        <section id="lectura" class="card" aria-label="Sección de Lectura">
          <div class="pad">
            <div class="sectionHead">
              <h2>📚 Lectura</h2>
              <p class="hint">Textos + preguntas (edítalos según tu clase)</p>
            </div>

            <ul class="list">
              <li class="item">
                <h3>Lectura 1: Crónica breve (Puerto Rico hoy)</h3>
                <p>
                  Objetivo: identificar tema, ideas principales, evidencia textual y punto de vista del autor.
                </p>
                <div class="meta">
                  <span class="tag">9.º</span>
                  <span class="tag">Comprensión</span>
                  <span class="tag">Evidencia</span>
                </div>
              </li>

              <li class="item">
                <h3>Lectura 2: Cuento corto (estructura narrativa)</h3>
                <p>
                  Objetivo: analizar inicio–nudo–desenlace, conflicto, personajes y ambiente.
                </p>
                <div class="meta">
                  <span class="tag">10.º</span>
                  <span class="tag">Narrativa</span>
                  <span class="tag">Análisis</span>
                </div>
              </li>

              <li class="item">
                <h3>Lectura 3: Artículo de opinión (argumentación)</h3>
                <p>
                  Objetivo: reconocer tesis, argumentos, contraargumentos y conectores lógicos.
                </p>
                <div class="meta">
                  <span class="tag">9.º–10.º</span>
                  <span class="tag">Argumentación</span>
                  <span class="tag">Conectores</span>
                </div>
              </li>
            </ul>

            <details>
              <summary>Actividades sugeridas <span>(lista rápida)</span></summary>
              <div class="twoCol">
                <div class="mini">
                  <h4>Antes de leer</h4>
                  <ul>
                    <li>Predice el tema a partir del título.</li>
                    <li>Define 5 palabras clave.</li>
                    <li>Pregunta guía: ¿Qué quiere lograr el autor?</li>
                  </ul>
                </div>
                <div class="mini">
                  <h4>Durante / Después</h4>
                  <ul>
                    <li>Subraya evidencia (cita + explicación).</li>
                    <li>Resume en 3–5 oraciones.</li>
                    <li>Escribe una conclusión personal (con respeto).</li>
                  </ul>
                </div>
              </div>
            </details>
          </div>
        </section>

        <!-- GRAMÁTICA -->
        <section id="gramatica" class="card" aria-label="Sección de Gramática">
          <div class="pad">
            <div class="sectionHead">
              <h2>🧠 Gramática</h2>
              <p class="hint">Reglas, ejemplos y práctica</p>
            </div>

            <details open>
              <summary>1) Clases de palabras <span>(sustantivo, verbo, adjetivo…)</span></summary>
              <p class="note">
                Practica: subraya el verbo principal y encierra el sujeto en 10 oraciones.
              </p>
              <div class="twoCol">
                <div class="mini">
                  <h4>Ejemplos</h4>
                  <ul>
                    <li><strong>Sustantivo:</strong> isla, cultura, estudiante</li>
                    <li><strong>Verbo:</strong> analiza, escribe, argumenta</li>
                    <li><strong>Adjetivo:</strong> caribeño/a, claro/a, preciso/a</li>
                  </ul>
                </div>
                <div class="mini">
                  <h4>Mini-práctica</h4>
                  <ul>
                    <li>Escribe 3 oraciones con adjetivos calificativos.</li>
                    <li>Cambia el tiempo verbal (presente → pasado).</li>
                  </ul>
                </div>
              </div>
            </details>

            <details>
              <summary>2) Sujeto y predicado <span>(simple y compuesto)</span></summary>
              <div class="twoCol">
                <div class="mini">
                  <h4>Regla</h4>
                  <ul>
                    <li>El <strong>sujeto</strong> concuerda con el verbo en número y persona.</li>
                    <li>El <strong>predicado</strong> incluye el verbo y sus complementos.</li>
                  </ul>
                </div>
                <div class="mini">
                  <h4>Ejemplo</h4>
                  <ul>
                    <li><strong>Los estudiantes</strong> <em>leen</em> textos diversos.</li>
                    <li><strong>María y José</strong> <em>presentan</em> su análisis.</li>
                  </ul>
                </div>
              </div>
            </details>

            <details>
              <summary>3) Conectores <span>(causa, contraste, conclusión)</span></summary>
              <div class="twoCol">
                <div class="mini">
                  <h4>Lista útil</h4>
                  <ul>
                    <li><strong>Causa:</strong> porque, ya que, debido a</li>
                    <li><strong>Contraste:</strong> sin embargo, no obstante, aunque</li>
                    <li><strong>Conclusión:</strong> por lo tanto, en conclusión</li>
                  </ul>
                </div>
                <div class="mini">
                  <h4>Actividad</h4>
                  <ul>
                    <li>Une 6 oraciones usando 6 conectores diferentes.</li>
                    <li>Revisa si cambia el significado.</li>
                  </ul>
                </div>
              </div>
            </details>
          </div>
        </section>

        <!-- ORTOGRAFÍA -->
        <section id="ortografia" class="card" aria-label="Sección de Ortografía">
          <div class="pad">
            <div class="sectionHead">
              <h2>✍️ Ortografía</h2>
              <p class="hint">Acentuación + signos + errores comunes</p>
            </div>

            <details open>
              <summary>1) Acentuación <span>(agudas, llanas, esdrújulas)</span></summary>
              <div class="twoCol">
                <div class="mini">
                  <h4>Reglas rápidas</h4>
                  <ul>
                    <li><strong>Agudas</strong> llevan tilde si terminan en <strong>n, s</strong> o <strong>vocal</strong>.</li>
                    <li><strong>Llanas</strong> llevan tilde si <em>NO</em> terminan en n, s o vocal.</li>
                    <li><strong>Esdrújulas</strong> siempre llevan tilde.</li>
                  </ul>
                </div>
                <div class="mini">
                  <h4>Ejemplos</h4>
                  <ul>
                    <li>Aguda: canción, café</li>
                    <li>Llena: árbol, lápiz</li>
                    <li>Esdrújula: música, rápido</li>
                  </ul>
                </div>
              </div>
            </details>

            <details>
              <summary>2) b / v, ll / y, g / j <span>(errores frecuentes)</span></summary>
              <div class="twoCol">
                <div class="mini">
                  <h4>Consejo</h4>
                  <ul>
                    <li>Haz una “lista personal” de tus 20 palabras que más confundes.</li>
                    <li>Practica con dictados cortos (1–2 min).</li>
                  </ul>
                </div>
                <div class="mini">
                  <h4>Mini-reto</h4>
                  <ul>
                    <li>Escribe 10 oraciones usando: viaje, lluvia, dibujo, gente, joven.</li>
                  </ul>
                </div>
              </div>
            </details>

            <details>
              <summary>3) Puntuación <span>(coma, punto y punto y coma)</span></summary>
              <div class="mini">
                <h4>Regla práctica</h4>
                <ul>
                  <li>Usa <strong>coma</strong> para separar ideas dentro de una oración.</li>
                  <li>Usa <strong>punto</strong> para cerrar una idea completa.</li>
                  <li>Usa <strong>punto y coma</strong> para unir ideas relacionadas, más fuerte que una coma.</li>
                </ul>
              </div>
            </details>
          </div>
        </section>

        <!-- RECURSOS -->
        <section id="recursos" class="card" aria-label="Sección de Recursos">
          <div class="pad">
            <div class="sectionHead">
              <h2>🧩 Recursos</h2>
              <p class="hint">Plantillas y recordatorios</p>
            </div>

            <ul class="list">
              <li class="item">
                <h3>Rúbrica básica de escritura (1 página)</h3>
                <p>Organización · Evidencia · Gramática · Ortografía · Vocabulario.</p>
                <div class="meta">
                  <span class="tag">Imprimible</span>
                  <span class="tag">9.º–10.º</span>
                </div>
              </li>
              <li class="item">
                <h3>Checklist de revisión antes de entregar</h3>
                <p>¿Tesis clara? ¿Citas? ¿Conectores? ¿Acentos? ¿Puntuación?</p>
                <div class="meta">
                  <span class="tag">Autocorrección</span>
                </div>
              </li>
              <li class="item">
                <h3>Calendario de tareas</h3>
                <p>Espacio para anunciar fechas, exámenes, proyectos y lecturas.</p>
                <div class="meta">
                  <span class="tag">Clase</span>
                </div>
              </li>
            </ul>

            <p class="note">
              Si quieres, puedo convertir esta página en: (1) una versión con “Unidad 1, 2, 3…”,
              (2) una versión para padres, o (3) una versión con tareas semanales.
            </p>
          </div>
        </section>
      </div>

      <div class="footer">
        <strong>Créditos de imágenes:</strong> Fotografías alojadas en Wikimedia Commons (uso libre según sus licencias).
        <br/>
        <strong>Edición:</strong> Puedes cambiar las imágenes reemplazando las URLs dentro del archivo.
      </div>
    </main>
  </div>

  <script>
    function buscar(){
      const q = document.getElementById("buscador").value.trim().toLowerCase();
      limpiar();
      if(!q) return;

      // Resalta coincidencias simples en títulos y párrafos
      const targets = document.querySelectorAll("h1,h2,h3,h4,p,li,summary");
      targets.forEach(el => {
        const text = el.textContent;
        const idx = text.toLowerCase().indexOf(q);
        if(idx >= 0){
          const before = text.slice(0, idx);
          const match = text.slice(idx, idx + q.length);
          const after  = text.slice(idx + q.length);
          el.innerHTML = `${escapeHtml(before)}<mark>${escapeHtml(match)}</mark>${escapeHtml(after)}`;
        }
      });
    }

    function limpiar(){
      // Restaura el contenido removiendo <mark> y reponiendo texto plano
      const marked = document.querySelectorAll("mark");
      if(marked.length === 0) return;

      const targets = document.querySelectorAll("h1,h2,h3,h4,p,li,summary");
      targets.forEach(el => {
        el.textContent = el.textContent; // quita marcas y HTML insertado
      });
    }

    function escapeHtml(str){
      return str
        .replaceAll("&","&amp;")
        .replaceAll("<","&lt;")
        .replaceAll(">","&gt;")
        .replaceAll('"',"&quot;")
        .replaceAll("'","&#039;");
    }
  </script>
</body>
</html>
# espanol
](https://tuusuario.github.io/espanol-9-10/
)
