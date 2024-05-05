<template>
  <v-app>
    <v-main>
      <v-row class="h-screen imagem align-center" id="home">
        <v-col class="px-16 text-center" md="6">
          <v-avatar
          class="mb-1"
          image="./assets/avatar.jpg"
          ></v-avatar>

          <h1>titulo</h1>

          <p class="paragrafo-1 mt-10 mb-10">The best commercial real estate in and around Buckville Park</p>

          <p class="paragrafo-2">We are a full-service brokerage firm in the Buckville Park area. Our team of experts is ready to help you with any questions you have.</p>
        </v-col>
        <v-col class="d-flex flex-column" md="6">
          <v-btn 
          class="w-25 mx-auto"
          color="botao"
          href="#sobreMim"
          >Sobre mim</v-btn>
          <v-btn 
          class="w-25 mx-auto mt-5"
          color="botao"
          href="#servicos"
          >Serviços</v-btn>
          <v-btn 
          class="w-25 mx-auto mb-5 mt-5"
          color="botao"
          href="#projetos"
          >Projetos</v-btn>
          <v-btn 
          class="w-25 mx-auto mb-5"
          color="botao"
          href="#empresa"
          >Empresa</v-btn>
          <v-btn 
          class="w-25 mx-auto"
          color="botao"
          href="#contatos"
          >Contatos</v-btn>
        </v-col>
      </v-row>

      <v-row class="h-screen align-center" id="sobreMim">
        <v-col class="px-16">
          <h1>Leticya Deffaveri</h1>

          <h2 class="mt-10 mb-10">Sobre mim (ela/dela)</h2>

          <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quos perferendis sed mollitia ipsam laborum deserunt distinctio a officia illum corrupti! Reprehenderit soluta est maiores corrupti sint illum, consequatur beatae nesciunt?</p>
        </v-col>
        <v-col>
          <v-img
          class="mx-auto"
          width="500"
          height="500"
          src="./assets/avatar.jpg"
          ></v-img>
        </v-col>
      </v-row>

      <v-row class="h-screen align-center" id="servicos">
        <v-col md="12">
          <h1>Coloque seu cabeçalho aqui!!!</h1>
        </v-col>

        <v-col md="3">
          <v-img></v-img>

          <h3>servico</h3>
          <p>descricao</p>
        </v-col>
      </v-row>
    </v-main>
  </v-app>
</template>

<script>
  //
</script>

<style>
  .imagem {
    background-image: url("./assets/home.jpg");
    background-size: cover;
  }

  #home, #sobreMim, #servicos {
    margin: 0px !important;
  }
  
  #home .v-btn {
    border: 2px solid #98713A;
  }

  .paragrafo-1 {
    font-size: 50px;
  }

  .paragrafo-2 {
    font-size: 15px;
  }

  #sobreMim h1 {
    text-decoration: underline 2px;
  }

</style>