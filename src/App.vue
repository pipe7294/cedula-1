<template>
  <div id="app">
    <div class="carnet">
      <aside>
        <div>
          <span>CEDULA DE INDENTIDAD</span>
          <img width="40" src="chile_bandera.png" alt="" />
        </div>

        <img src="yo.png" alt="" />
        <p>RUN {{ RUN }}</p>
      </aside>

      <main>
        <header>
          <p>REPUBLICA DE CHILE</p>
          <span>SERVICIO DE REGISTRO CIVIL E IDENTIFICACIÓN</span>
        </header>
        <section>
          <article>
            <header>APELLIDOS</header>
            <span>{{ APELLIDOS }}</span>
          </article>
          <article>
            <header>NOMBRES</header>
            <span>{{NOMBRES}}</span>
          </article>

          <div class="grid-2-colums">
            <article>
              <header>NACIONALIDAD</header>
              <span>{{NACIONALIDAD}}</span>
            </article>
            <article>
              <header>SEXO</header>
              <span>{{SEXO}}</span>
            </article>
          </div>
          <div class="grid-2-colums">
            <article>
              <header>FECHA DE NACIMIENTO</header>
              <span>{{FECHANACIMIENTO}}</span>
            </article>
            <article>
              <header>NUMERO DOCUMENTO</header>
              <span>{{NUMERODOCUMENTO}}</span>
            </article>
          </div>
          <div class="grid-2-colums">
            <article>
              <header>FECHA DE EMISION</header>
              <span>{{FECHAEMISION}}</span>
            </article>
            <article>
              <header>FECHA DE VENCIMIENTO</header>
              <span>{{FECHAVENCIMIENTO}}</span>
            </article>
          </div>
          <article>
            <header>FIRMA DEL TITULAR</header>
            <span><img src="Mi_firma.png" width="60"></span>
          </article>
        </section>
      </main>
    </div>
  </div>

</template>

<script>


export default {
  name: 'App',
  data() {
    return {
      RUN: "17979614-7",
      APELLIDOS: "CARMONA MATURANA",
      NOMBRES: "FELIPE EDUARDO",
      NACIONALIDAD: "CHILENA",
      SEXO: "MASCULINO",
      FECHANACIMIENTO: "30/09/1991",
      NUMERODOCUMENTO: "155.485.457",
      FECHAEMISION: "03 MAR 2015",
      FECHAVENCIMIENTO: "30 SEPT 2021"
    }
  }
    
}
</script>

<style>
body {
        display: flex;
        justify-content: center;
        align-items: center;
        height: 60vh;
        font-size: 10px;
        font-family: sans-serif;
      }

      .carnet {
        width: 400px;
        height: 230px;
        background: #c8deed;
        border-radius: 20px;
        display: grid;
        grid-template-columns: 30% 1fr;
        padding: 15px;
        box-shadow: 0px 0px 10px 2px black;
      }

      aside div {
        display: flex;
      }

      aside > img {
        margin-top: 15px;
        width: 100%;
      }

      aside p {
        text-align: center;
        font-size: 12px;
        font-weight: bold;
      }

      main {
        padding: 0px 14px;
      }

      main article {
        margin: 4px 0px;
      }

      main article header {
        font-weight: bold;
        color: #0235a4;
        font-size: 8px;
      }

      main header p {
        font-size: 20px;
        margin: 0;
        font-weight: bold;
        color: #0235a4;
      }

      main header span {
        font-size: 8px;
        color: #399be1;
      }

      main section {
        margin-top: 10px;
      }

      main section article span {
        font-size: 13px;
        font-weight: 600;
      }

      main section .grid-2-colums {
        display: grid;
        grid-template-columns: 50% 50%;
      }
</style>
