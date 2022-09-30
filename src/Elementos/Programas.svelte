<script>
    import Niveles from "./Niveles.svelte";
    import Certificaciones from "./Certificaciones.svelte";

let boton=false;

function Activo(){
  boton=!boton;
}

</script>

<Niveles/>
<div class="fondo">
<h1 class="titulo"><b> Proyectos realizados</b></h1>

<section class="layout">
  <div class="centro">
    <div class="card"  style="width: 90%; height: 90%;">
      <img src="peliculas.jpg" class="card-img-top" alt="..." />
      <div class="card-body">
        <h5 class="card-title">Conexion api peliculas</h5>
        <p class="card-text">Proyecto svelte-javascript donde se muestra el catalogo de peliculas, descripciones y puntuación de estas.</p>
        <a href="/" class="btn btn-primary">Ver GitHub</a>
      </div>
    </div>
  </div>
  <div class="centro">
    <div class="card" style="width: 90%; height: 90%;">
      <img src="cajero.jpg" class="card-img-top" alt="..." />
      <div class="card-body">
        <h5 class="card-title">Cajero java</h5>
        <p class="card-text">En este proyecto se simula el funcionamiento de un cajero en java del lado del backend <br> <br></p>
        <a href="/" class="btn btn-primary">Ir a GitHub</a>
      </div>
    </div>
  </div>
  <div class="centro">
    <div class="card"  style="width: 90%; height: 90%;">
      <img src="chat.png" class="card-img-top" alt="..." />
      <div class="card-body">
        <h5 class="card-title">Chat de una tienda con accesos</h5>
        <p class="card-text">Se muestra el funcionamiento de un chat online con java y sus partes funcionales como los privilegios <br><br></p>
        <a href="/" class="btn btn-primary">Ir a GitHub</a>
      </div>
    </div>
  </div>
  <div class="centro">
    <div class="card"  style="width: 90%; height: 90%;">
      <img src="vacunas.png" class="card-img-top" alt="..." />
      <div class="card-body">
        <h5 class="card-title">Vacunas covis</h5>
        <p class="card-text">En este proyecto se muestra las funcionalidades de caracteristicas de las vacunas contra covid.</p>
        <a href="/" class="btn btn-primary">Ir a GitHub</a>
      </div>
    </div>
  </div>
  <div class="centro">
    <div class="card"  style="width: 90%; height: 90%;">
      <img src="tienda.png" class="card-img-top" alt="..." />
      <div class="card-body">
        <h5 class="card-title">Ventas de una tienda con c#</h5>
        <p class="card-text">En este proyecto se implementan funciones como la de un cajero comercial para el cobro de prendas.</p>
        <a href="/" class="btn btn-primary">Ir a GitHub</a>
      </div>
    </div>
  </div>
  <div class="centro">
    <div class="card"  style="width: 90%; height: 90%;">
      <img src="cv.png" class="card-img-top" alt="..." />
      <div class="card-body">
        <h5 class="card-title">CV.</h5>
        <p class="card-text">Este proyecto es el que se encuentra la implementación de esta pagina web donde se muestran los portafolios y caracteristics mias. <br><br><br><br></p>
        <a href="/" class="btn btn-primary">Ir a GitHub</a>
      </div>
    </div>
  </div>
</section>
<br>
<br>
<button type="button" class="btn btn-info" on:click={Activo}>Ver certificaciones extras</button>

<div>
  
  {#if boton}
  <Certificaciones/>
  <br>
  <br>
  {/if}
</div>
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
  background-image: url("https://portafolio-entj.vercel.app/imagenAbajo.jpg");
  background-repeat: no-repeat;
    background-size: cover;
    background-attachment: fixed;
    background-position: center;

}
</style>
