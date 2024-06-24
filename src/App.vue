<template>
  <div class="carnet">
    <aside>
      <div>
        <span>CEDULA DE INDENTIDAD</span>
        <img width="40" src="./assets/images/chile_bandera.png" alt="" />
      </div>
      <v-container fluid>
      <img  class="image" src="./assets/images/foto_elon.jpg" alt="">
    </v-container>
      <p>{{ run }}</p>
    </aside>

    <main>
      <header>
        <p>REPUBLICA DE CHILE</p>
        <span>SERVICIO DE REGISTRO CIVIL E IDENTIFICACIÓN</span>
      </header>
      <section>
        <article>
          <header>APELLIDOS</header>
          <span>{{ apellidos }}</span>
        </article>
        <article>
          <header>NOMBRES</header>
          <span>{{nombres}}</span>
        </article>

        <div class="grid-2-colums">
          <article>
            <header>NACIONALIDAD</header>
            <span>{{nacionalidad}}</span>
          </article>
          <article>
            <header>SEXO</header>
            <span>{{ sexo }}</span>
          </article>
        </div>
        <div class="grid-2-colums">
          <article>
            <header>FECHA DE NACIMIENTO</header>
            <span>{{ fechadenacimiento }} </span>
          </article>
          <article>
            <header>NÙMERO DOCUMENTO</header>
            <span>{{ numerodedocumento }}</span>
          </article>
        </div>
        <div class="grid-2-colums">
          <article>
            <header>FECHA DE EMISIÒN</header>
            <span>{{ fechadeemision }}</span>
          </article>
          <article>
            <header>FECHA DE VENCIMIENTO</header>
            <span>{{ fechadevencimiento }}</span>
          </article>
        </div>
        <article>
          <header>FIRMA DEL TITULAR</header>
          <span>{{ firmadeltitular }}</span>
        </article>
      </section>
    </main>
  </div>

</template>

<script>
export default {
  name: 'App',
  data() {
    return {
  
      run: "22.222.222-2",
      apellidos: "MUSK",
      nombres: "ELON REEVE",
      nacionalidad: "SUDAFRICANO",
      sexo: "M",
      fechadenacimiento: "28 JUN 1971",
      numerodedocumento: "222.222.222",
      fechadeemision: "01 ENE 2025",
      fechadevencimiento: "30 ENE 2030",
      firmadeltitular: "X Æ A-12",

    };
  }
};

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

aside>img {
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
.image{
  width: 100px;
  padding-top: 20px;
}
</style>
