<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <title>Craft Market – English Project</title>
  <meta name="viewport" content="width=device-width, initial-scale=1" />

  <style>
    /* ====== ESTILO GENERAL – LOOK MINECRAFT/PIXEL ====== */
    :root {
      --green-main: #6ca332;
      --green-dark: #3f5f1b;
      --brown-main: #8b5a2b;
      --cream: #f4f0da;
      --panel-bg: rgba(248, 244, 224, 0.95);
      --border-pixel: 4px;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      font-family: "Courier New", monospace;
      background-color: #7ec850;
      color: #222;
      min-height: 100vh;
      /* Pattern background */
      background-image:
        linear-gradient(90deg, rgba(0,0,0,0.08) 1px, transparent 1px),
        linear-gradient(180deg, rgba(0,0,0,0.08) 1px, transparent 1px);
      background-size: 40px 40px;
    }

    a {
      color: #1b4a9f;
      text-decoration: none;
      font-weight: bold;
    }

    a:hover {
      text-decoration: underline;
    }

    .page-wrapper {
      max-width: 1100px;
      margin: 0 auto;
      padding: 1.5rem 1rem 3rem;
    }

    /* ====== CABECERA ====== */
    header {
      background: var(--panel-bg);
      border: var(--border-pixel) solid var(--green-dark);
      box-shadow: 0 0 0 var(--border-pixel) #000;
      padding: 1.5rem 1rem;
      margin-bottom: 1.5rem;
      text-align: center;
    }

    header h1 {
      font-size: 1.8rem;
      text-transform: uppercase;
      letter-spacing: 2px;
      margin-bottom: 0.5rem;
    }

    header p {
      font-size: 0.9rem;
      line-height: 1.4;
    }

    /* ====== NAV ====== */
    .grade-nav {
      margin-top: 1rem;
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 0.75rem;
    }

    .grade-btn {
      background: var(--green-main);
      border: var(--border-pixel) solid var(--green-dark);
      box-shadow: 0 0 0 var(--border-pixel) #000;
      color: #fff;
      padding: 0.65rem 1.2rem;
      font-size: 0.9rem;
      text-transform: uppercase;
      cursor: pointer;
      text-decoration: none;
      display: inline-block;
    }

    .grade-btn:hover {
      background: #7fbf3f;
      transform: translateY(-2px);
      text-decoration: none;
    }

    /* ====== SECCIONES POR GRADO ====== */
    section {
      background: var(--panel-bg);
      border: var(--border-pixel) solid var(--brown-main);
      box-shadow: 0 0 0 var(--border-pixel) #000;
      padding: 1.5rem 1rem;
      margin-bottom: 1.5rem;
      scroll-margin-top: 20px;
    }

    section h2 {
      font-size: 1.4rem;
      margin-bottom: 0.4rem;
    }

    section h3 {
      font-size: 1rem;
      margin: 0.8rem 0 0.4rem;
      text-transform: uppercase;
    }

    .tagline {
      font-size: 0.85rem;
      color: #555;
      margin-bottom: 0.8rem;
    }

    .flex-row {
      display: flex;
      flex-wrap: wrap;
      gap: 1rem;
      margin-top: 0.7rem;
    }

    .panel {
      flex: 1 1 260px;
      background: #fffdf5;
      border: 3px solid #d3c9a3;
      padding: 0.75rem;
    }

    .panel p {
      font-size: 0.9rem;
      line-height: 1.4;
    }

    .panel ul {
      margin-left: 1.1rem;
      margin-top: 0.3rem;
      font-size: 0.9rem;
    }

    .panel li {
      margin-bottom: 0.2rem;
    }

    .craft-image,
    .card-image {
      width: 100%;
      max-width: 480px;
      border: 4px solid #000;
      display: block;
      margin: 0 auto;
    }

    .media-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
      gap: 1rem;
      margin-top: 0.8rem;
    }

    /* === CONTENEDOR PARA SHORTS VERTICALES === */
    .short-wrapper {
      width: 100%;
      max-width: 360px;      /* tamaño tipo celular */
      margin: 0 auto;
      border: 4px solid #000;
      box-shadow: 0 0 0 4px #000;
      overflow: hidden;
    }

    .short-wrapper iframe {
      width: 100%;
      aspect-ratio: 9 / 16;  /* vertical */
      border: none;
      display: block;
    }

    .gallery-link {
      display: inline-block;
      background: var(--green-main);
      color: white;
      padding: 0.6rem 1rem;
      border: 3px solid var(--green-dark);
      margin-top: 0.5rem;
      font-weight: bold;
    }

    .gallery-link:hover {
      background: #7fbf3f;
      text-decoration: none;
    }

    /* ====== FOOTER ====== */
    footer {
      text-align: center;
      font-size: 0.75rem;
      color: #222;
      padding-top: 0.5rem;
    }

    @media (min-width: 900px) {
      header h1 {
        font-size: 2.1rem;
      }
    }
  </style>
</head>

<body>
  <div class="page-wrapper">
    <header>
      <h1>Craft Market – English Project</h1>
      <p>
        Minecraft-style gallery for our <strong>Artisan Market</strong>.<br />
        Choose a grade to see the craft, materials, conversation card, story and video.
      </p>

      <nav class="grade-nav">
        <a class="grade-btn" href="#grade2">2º Grade / 2º Grado</a>
        <a class="grade-btn" href="#grade3">3º Grade / 3º Grado</a>
        <a class="grade-btn" href="#grade4">4º Grade / 4º Grado</a>
      </nav>
    </header>

    <section id="grade2">
      <h2>Grade 2 – Hand-Painted Napkin & Bottle Piggy Bank</h2>
      <p class="tagline">Servilleta pintada a mano y alcancía con botella reciclada.</p>

      <div class="flex-row">
        <div class="panel">
          <h3>Craft & Materials</h3>
          <img
            src="https://files.manuscdn.com/user_upload_by_module/session_file/310419663026807096/tvqyNcNKHbqBHzdg.png"
            alt="Hand-painted napkin and bottle piggy bank with labeled materials"
            class="craft-image"
          />
          <p style="margin-top:0.5rem;">
            Parents can see the final craft and the basic materials:
          </p>
          <ul>
            <li><strong>Napkin / cloth fabric</strong></li>
            <li><strong>Fabric paint</strong></li>
            <li><strong>Brush</strong></li>
            <li><strong>Plastic bottle</strong></li>
          </ul>
        </div>

        <div class="panel">
          <h3>Conversation Card</h3>
          <img
            src="https://files.manuscdn.com/user_upload_by_module/session_file/310419663026807096/QKNJBnwssgIBOtZD.jpg"
            alt="Grade 2 conversation card"
            class="card-image"
          />
          <p style="margin-top:0.5rem;">
            Short dialogue to practice buying and selling: <br />
            <em>Hello! – What is it? – How much is it? – Here you are – Thank you!</em>
          </p>
        </div>
      </div>

      <div class="media-grid">
        <div class="panel">
          <h3>Storybook</h3>
          <p>
            Read our story <strong>"Roblox Craft Market Day!"</strong> with your child to see the
            market interactions in context.
          </p>
          <p style="margin-top:0.4rem;">
            <a href="https://gemini.google.com/share/30ff85d946a1" target="_blank">
              📖 Open the storybook
            </a>
          </p>
        </div>

        <div class="panel">
          <h3>Practice Video</h3>
          <div class="short-wrapper">
            <iframe
              src="https://www.youtube.com/embed/axvpfnw32to"
              title="Craft Market – Conversation Practice"
              allowfullscreen
            ></iframe>
          </div>
          <p style="margin-top:0.4rem;">
            Watch the video and pause to repeat each line with your child.
          </p>
        </div>

        <div class="panel">
          <h3>Class Gallery</h3>
          <p>
            See photos of students working and their crafts.
          </p>
          <a href="https://photos.app.goo.gl/Jnex28iRAQafVxed9" target="_blank" class="gallery-link">
            📸 View Grade 2 Photos
          </a>
        </div>
      </div>
    </section>

    <section id="grade3">
      <h2>Grade 3 – Dreamcatchers</h2>
      <p class="tagline">Atrapasueños con estambre de lana y palitos de madera.</p>

      <div class="flex-row">
        <div class="panel">
          <h3>Craft & Materials</h3>
          <img
            src="https://files.manuscdn.com/user_upload_by_module/session_file/310419663026807096/SqCUYkxMLpIkehWM.png"
            alt="Dreamcatcher with labeled materials"
            class="craft-image"
          />
          <p style="margin-top:0.5rem;">
            Main materials:
          </p>
          <ul>
            <li><strong>Yarn / estambre</strong></li>
            <li><strong>Wooden sticks / palitos de madera</strong></li>
            <li><strong>Thread / hilo</strong></li>
            <li><strong>Beads and feathers</strong></li>
            <li><strong>Glue</strong></li>
          </ul>
        </div>

        <div class="panel">
          <h3>Conversation Card</h3>
          <img
            src="https://files.manuscdn.com/user_upload_by_module/session_file/310419663026807096/HCCmodMiExfiCpEz.jpg"
            alt="Grade 3 conversation card"
            class="card-image"
          />
          <p style="margin-top:0.5rem;">
            Color & price practice: <br />
            <em>Can I help you? – What colors do you have? – I like the blue one. – How much does it cost?</em>
          </p>
        </div>
      </div>

      <div class="media-grid">
        <div class="panel">
          <h3>Storybook</h3>
          <p>
            The same storybook supports all grades, but third graders focus on
            <strong>colors</strong> and <strong>polite questions</strong>.
          </p>
          <p style="margin-top:0.4rem;">
            <a href="https://gemini.google.com/share/30ff85d946a1" target="_blank">
              📖 Open the storybook
            </a>
          </p>
        </div>

        <div class="panel">
          <h3>Practice Video</h3>
          <div class="short-wrapper">
            <iframe
              src="https://www.youtube.com/embed/axvpfnw32to"
              title="Craft Market – Conversation Practice"
              allowfullscreen
            ></iframe>
          </div>
          <p style="margin-top:0.4rem;">
            Use the pauses in the video to repeat the buying/selling dialogue.
          </p>
        </div>

        <div class="panel">
          <h3>Class Gallery</h3>
          <p>
            See photos of Grade 3 students weaving and decorating their dreamcatchers.
          </p>
          <a href="https://photos.app.goo.gl/t7oNCMs5RCzU1Ubx8" target="_blank" class="gallery-link">
            📸 View Grade 3 Photos
          </a>
        </div>
      </div>
    </section>

    <section id="grade4">
      <h2>Grade 4 – Alebrijes & Paper Airplanes</h2>
      <p class="tagline">
        Alebrijes con arcilla o porcelana fría y aviones de papel decorados.
      </p>

      <div class="flex-row">
        <div class="panel">
          <h3>Craft & Materials</h3>
          <img
            src="https://files.manuscdn.com/user_upload_by_module/session_file/310419663026807096/YleJXRdSfBmPNYfx.png"
            alt="Alebrije and paper airplane with labeled materials"
            class="craft-image"
          />
          <p style="margin-top:0.5rem;">
            Some of the materials students may use:
          </p>
          <ul>
            <li><strong>Clay or cold porcelain</strong></li>
            <li><strong>Paints & brushes</strong></li>
            <li><strong>Water</strong></li>
            <li><strong>Thread / yarn / beads / wire</strong></li>
            <li><strong>Cardstock paper for airplanes</strong></li>
          </ul>
        </div>

        <div class="panel">
          <h3>Conversation Card</h3>
          <img
            src="https://files.manuscdn.com/user_upload_by_module/session_file/310419663026807096/rHEWJmOuzUTgrtru.jpg"
            alt="Grade 4 conversation card"
            class="card-image"
          />
          <p style="margin-top:0.5rem;">
            Longer interaction about <strong>colors</strong>, <strong>patterns</strong> and choosing a gift.
          </p>
        </div>
      </div>

      <div class="media-grid">
        <div class="panel">
          <h3>Storybook</h3>
          <p>
            Fourth grade connects the story with <strong>Mexican folk art (alebrijes)</strong>
            and more complex dialogues.
          </p>
          <p style="margin-top:0.4rem;">
            <a href="https://gemini.google.com/share/30ff85d946a1" target="_blank">
              📖 Open the storybook
            </a>
          </p>
        </div>

        <div class="panel">
          <h3>Practice Video</h3>
          <div class="short-wrapper">
            <iframe
              src="https://www.youtube.com/embed/axvpfnw32to"
              title="Craft Market – Conversation Practice"
              allowfullscreen
            ></iframe>
          </div>
          <p style="margin-top:0.4rem;">
            Families can watch and practice the dialogues at home.
          </p>
        </div>

        <div class="panel">
          <h3>Class Gallery</h3>
          <p>
            See photos of Grade 4 students modeling alebrijes and testing their paper planes.
          </p>
          <a href="https://photos.app.goo.gl/AvHfXeNcYSACvpGe9" target="_blank" class="gallery-link">
            📸 View Grade 4 Photos
          </a>
        </div>
      </div>
    </section>

    <footer>
      English Craft Market Project – Instituto San Felipe Bacalar
    </footer>
  </div>
</body>
</html>

    <footer>
      English Craft Market Project – Instituto San Felipe Bacalar
    </footer>
  </div>
</body>
</html>
