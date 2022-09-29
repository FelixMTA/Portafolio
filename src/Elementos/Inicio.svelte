<script>
  import Programas from "./Programas.svelte";
</script>

<body>
  <section class="layout">
    <div class="sidebar">
      <div class="centrar">
        <img
          src="https://portafolio-entj.vercel.app/ima.jpg"
          alt="imagen"
          class="circulo"
        />
      </div>
      <div class="centro">
        <div class="card text-center">
          <div class="card-header color:primary "><b>Programador</b></div>
          <div class="card-body">
            <h4 class="card-title">Felix Santiago Martínez Pérez</h4>
            <h5 class="card-title">22/Enero/1997</h5>
            <h5 class="card-title">felixmtz@pm.me</h5>
          </div>
          <div class="card-footer text-muted">
            <button type="button" class="btn btn-info">Ver Cv.</button>
          </div>
        </div>
      </div>
    </div>

    <div class="body">
      <div class="parrafos">
        <h1><b>Programador</b></h1>
        <h3>
          Mi nombre es Félix Santiago Martínez Pérez me interesa el desarrollo de
          funcionalidades que den soluciones a problemas de la vida diaria y
          laboral.
        </h3>
        <h3>
          En este momento he realizado trabajos como se muestran en mi
          portafolio con ello he ganando experiencia y un interés a seguir mejorando cada día más.
        </h3>
      </div>
    </div>
  </section>
</body>

<Programas />

<style>
  body {
    background-image: url("https://portafolio-entj.vercel.app/fractal.jpg");
    background-repeat: no-repeat;
    background-size: cover;
    background-attachment: fixed;
    background-position: center;
  }
  .layout {
    width: 100%;
    min-width: 500px;
    display: grid;
    grid:
      "sidebar body" 1fr
      / 35% 65%;
    gap: 8px;
  }

  .sidebar {
    grid-area: sidebar;
  }
  .body {
    grid-area: body;
  }

  .circulo {
    width: 60%;
    height: 60%;
    -moz-border-radius: 50%;
    -webkit-border-radius: 50%;
    border-radius: 50%;
    background: #9da49d;
    margin: 10%;
  }

  .centro {
    width: 80%;
    margin: auto;
  }

  .sidebar {
    justify-content: center;
    text-align: center;
  }
  .parrafos {
    color: rgb(16, 16, 17);
    margin: 20%;
    text-align: center;
    -webkit-text-stroke: 0.6px rgb(211, 227, 230);
  }
  
</style>
