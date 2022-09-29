<script>
    import Niveles from "./Niveles.svelte";
</script>

<Niveles/>
<div class="fondo">
<h1 class="titulo"><b> Proyectos realizados</b></h1>

<section class="layout">
  <div class="centro">
    <div class="card"  style="width: 90%; height: 90%;">
      <img src="https://portafolio-entj.vercel.app/s.jpeg" class="card-img-top" alt="..." />
      <div class="card-body">
        <h5 class="card-title">Nombre de proyecto</h5>
        <p class="card-text">Contenido del proyecto</p>
        <a href="/" class="btn btn-primary">Ver GitHub</a>
      </div>
    </div>
  </div>
  <div class="centro">
    <div class="card" style="width: 90%; height: 90%;">
      <img src="https://portafolio-entj.vercel.app/s.jpeg" class="card-img-top" alt="..." />
      <div class="card-body">
        <h5 class="card-title">Nombre de proyecto</h5>
        <p class="card-text">Contenido del proyecto</p>
        <a href="/" class="btn btn-primary">Ir a GitHub</a>
      </div>
    </div>
  </div>
  <div class="centro">
    <div class="card"  style="width: 90%; height: 90%;">
      <img src="https://portafolio-entj.vercel.app/s.jpeg" class="card-img-top" alt="..." />
      <div class="card-body">
        <h5 class="card-title">Nombre de proyecto</h5>
        <p class="card-text">Contenido del proyecto</p>
        <a href="/" class="btn btn-primary">Ir a GitHub</a>
      </div>
    </div>
  </div>
  <div class="centro">
    <div class="card"  style="width: 90%; height: 90%;">
      <img src="https://portafolio-entj.vercel.app/s.jpeg" class="card-img-top" alt="..." />
      <div class="card-body">
        <h5 class="card-title">Nombre de proyecto</h5>
        <p class="card-text">Contenido del proyecto</p>
        <a href="/" class="btn btn-primary">Ir a GitHub</a>
      </div>
    </div>
  </div>
  
</section>
</div>
<style>
  .layout {
    display: grid;
    grid-template-rows: repeat(2, 1fr);
    grid-template-columns: repeat(3, 1fr);
    gap: 8px;
   
   
   
  }
.centro{
    display: flex;
    justify-content: center;
    align-items: center;
}
.titulo{

text-align: center;

margin: 0%;
background-color: rgba(255, 255, 255, 0.397);

}
.fondo{
  background-image: url("./imagenAbajo.jpg");
  background-repeat: no-repeat;
    background-size: cover;
    background-attachment: fixed;
    background-position: center;

}
</style>
