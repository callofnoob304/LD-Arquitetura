<template>
  <v-app>
    <v-main>
      <v-row class="h-screen imagem align-center" id="home">
        <v-col class="px-16 text-center text-white" md="6">
          <v-avatar
          class="mb-1"
          image="./assets/homePage/logoEmpresa.jpg"
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

      <v-row class="h-screen align-center bg-red" id="sobreMim">
        <v-col class="px-16">
          <h1 class="text-center">Leticya Deffaveri</h1>

          <h2 class="mt-10 mb-10">Sobre mim (ela/dela)</h2>

          <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quos perferendis sed mollitia ipsam laborum deserunt distinctio a officia illum corrupti! Reprehenderit soluta est maiores corrupti sint illum, consequatur beatae nesciunt?</p>
        </v-col>
        <v-col>
          <v-img
          class="mx-auto"
          width="500"
          height="500"
          src="./assets/homePage/logoEmpresa.jpg"
          ></v-img>
        </v-col>
      </v-row>

      <v-row class="h-screen justify-center align-center" id="servicos">
        <v-col class="text-center" md="10">
          <h1 class="mb-10">Lorem ipsum dolor sit amet consectetur adipisicing elit. Maiores neque fugit, ratione hic vitae quibusdam quia voluptas enim veniam totam reiciendis odit doloremque praesentium repudiandae eos aperiam voluptatum atque dolorem?</h1>

          <v-card class="bg-cyan" flat>
            <v-window v-model="window">
              <v-window-item :value="1">
                <v-row class="justify-center py-5">
                  <v-col class="d-flex justify-center" md="3">
                    <v-card width="300" flat elevation="8">
                      <v-img
                      src="./assets/servicos/reforma.jpg"
                      ></v-img>
                      <v-card-text class="text-center">
                        <h3 class="mb-2">Reforma</h3>
                        <p>descrição</p>
                      </v-card-text>
                    </v-card>
                  </v-col>
                  <v-col class="d-flex justify-center" md="3">
                    <v-card width="300" flat elevation="8">
                      <v-img
                      src="./assets/servicos/reforma.jpg"
                      ></v-img>
                      <v-card-text class="text-center">
                        <h3 class="mb-2">Reforma</h3>
                        <p>descrição</p>
                      </v-card-text>
                    </v-card>
                  </v-col>
                  <v-col class="d-flex justify-center" md="3">
                    <v-card width="300" flat elevation="8">
                      <v-img
                      src="./assets/servicos/reforma.jpg"
                      ></v-img>
                      <v-card-text class="text-center">
                        <h3 class="mb-2">Reforma</h3>
                        <p>descrição</p>
                      </v-card-text>
                    </v-card>
                  </v-col>
                </v-row>
              </v-window-item>
              <v-window-item :value="2">
                <v-row class="justify-center py-5">
                  <v-col class="d-flex justify-center" md="3">
                    <v-card width="300" flat elevation="8">
                      <v-img
                      src="./assets/servicos/reforma.jpg"
                      ></v-img>
                      <v-card-text class="text-center">
                        <h3 class="mb-2">Reforma</h3>
                        <p>descrição</p>
                      </v-card-text>
                    </v-card>
                  </v-col>
                  <v-col class="d-flex justify-center" md="3">
                    <v-card width="300" flat elevation="8">
                      <v-img
                      src="./assets/servicos/reforma.jpg"
                      ></v-img>
                      <v-card-text class="text-center">
                        <h3 class="mb-2">Reforma</h3>
                        <p>descrição</p>
                      </v-card-text>
                    </v-card>
                  </v-col>
                  <v-col class="d-flex justify-center" md="3">
                    <v-card width="300" flat elevation="8">
                      <v-img
                      src="./assets/servicos/reforma.jpg"
                      ></v-img>
                      <v-card-text class="text-center">
                        <h3 class="mb-2">Reforma</h3>
                        <p>descrição</p>
                      </v-card-text>
                    </v-card>
                  </v-col>
                </v-row>
              </v-window-item>
            </v-window>
            <v-card-actions class="justify-center">
              <v-pagination
                v-model="window"
                :length="2"
                :total-visible="2"
                rounded
                next-icon="mdi-menu-right"
                prev-icon="mdi-menu-left"
              ></v-pagination>
            </v-card-actions>
          </v-card>
        </v-col>
      </v-row>

      <v-row class="h-screen justify-center align-center">
        <v-col class="text-center">
          <h1 class="mb-5">Projetos</h1>

          <v-row class="mb-5 justify-center">
            <v-col md="3">
              <v-img class="cursor" src="./assets/projetos/foto1/projeto1.webp" @click="abrirFoto('foto1')"/>
              <v-divider class="mb-5 mt-5" color="#000"></v-divider>
              <h3>teste askjhdalksjd</h3>
              <h2>teste askjhdalksjd</h2>
              <h4>teste askjhdalksjd</h4>
              <v-divider class="mb-5 mt-5" color="#000"></v-divider>
            </v-col>
            <v-col md="3">
              <v-img class="cursor" src="./assets/projetos/foto2/projeto2.webp" @click="abrirFoto('foto2')"/>
              <v-divider class="mb-5 mt-5" color="#000"></v-divider>
              <h3>teste askjhdalksjd</h3>
              <h2>teste askjhdalksjd</h2>
              <h4>teste askjhdalksjd</h4>
              <v-divider class="mb-5 mt-5" color="#000"></v-divider>
            </v-col>
            <v-col md="3">
              <v-img class="cursor" src="./assets/projetos/foto3/projeto3.webp" @click="abrirFoto('foto3')"/>
              <v-divider class="mb-5 mt-5" color="#000"></v-divider>
              <h3>teste askjhdalksjd</h3>
              <h2>teste askjhdalksjd</h2>
              <h4>teste askjhdalksjd</h4>
              <v-divider class="mb-5 mt-5" color="#000"></v-divider>
            </v-col>
          </v-row>
        </v-col>
      </v-row>

      <v-dialog v-model="dialog" width="1000">
        <v-card>
          <v-row>
            <v-col>
              <v-carousel>
                <v-carousel-item
                v-for="(image, index) in imagensAtuais"
                :key="index"
                :src="image"
                cover
                ></v-carousel-item>
              </v-carousel>
            </v-col>
          </v-row>
        </v-card>
      </v-dialog>
    </v-main>
  </v-app>
</template>

<!-- utilizar v-window para os cards de servicos e v-carrosel para o show de slides dos projetos!! -->

<script>
  export default {
    name: 'WebSite LD-Aquitetura',

    data() {
      return {
        window: 1,
        dialog: false,
        imagensAtuais: [],
        imagens: {
          foto1: [
            "./assets/projetos/foto1/projeto1.webp",
            "./assets/projetos/foto1/projeto1.webp",
            "./assets/projetos/foto1/projeto1.webp",
          ],
          foto2: [
            "./assets/projetos/foto2/projeto2.webp",
            "./assets/projetos/foto2/projeto2.webp",
            "./assets/projetos/foto2/projeto2.webp",
          ],
          foto3: [
            "./assets/projetos/foto3/projeto3.webp",
            "./assets/projetos/foto3/projeto3.webp",
            "./assets/projetos/foto3/projeto3.webp",
          ],
        },
      }
    },

    methods: {
      abrirFoto(foto) {
        this.imagensAtuais = this.imagens[foto];
        this.dialog = true;
      }
    },
  } 
</script>

<style>
  .imagem {
    background-image: url("./assets/homePage/homeFundo.jpg");
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

  .cursor {
    cursor: pointer;
  }
</style>