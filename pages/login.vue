<template>
  <div
    class="light-blue lighten-5"
    style="height: 100vh; background-color: #dde7ed"
  >
    <v-container class="pt-0">

      <v-row class="pr-6" justify="center" align="center">
        <v-col cols="8" class="pa-12" align="center">
          <v-card max-width="600px" elevation="0" tile color="transparent">

            <v-card-text>
              <v-row class="pb-12">
                <v-col cols="12" class="pb-0">
                  <v-img src="/logo_azul.svg" style="height: 132px; width: 162px"></v-img>
                </v-col>
              </v-row>
              <v-row>
                <v-col cols="12" class="pb-0">
                  <v-text-field
                    label="Email"
                    outlined
                    background-color="#FBFEFF"
                    :rules="[ val => val && val.length <12  || 'CPF inválido!']"
                  ></v-text-field>
                </v-col>

              </v-row>

              <v-row>
                <v-col cols="12" class="pt-0 pb-0">
                  <v-text-field
                    label="Senha"
                    outlined
                    background-color="#FBFEFF"
                  ></v-text-field>
                </v-col>
              </v-row>

              <v-row>
                <v-col cols="9" style="text-align: left">
                  <span class="primary--text">
                    Esqueci minha senha
                  </span>
                </v-col>

                <v-col cols="3">
                  <v-btn
                    rounded
                    depressed
                    color="primary"
                    to="/cadastro-dois"
                    nuxt
                  >
                    Acessar
                  </v-btn>
                </v-col>
              </v-row>

              <v-row class="pt-6">
                <v-col cols="12" style="text-align: right">
                  <span class="primary--text">
                    Não possui acesso?
                  </span>
                  <span class="primary--text font-weight-bold">
                    Cadastre-se aqui
                  </span>
                </v-col>
              </v-row>

            </v-card-text>
          </v-card>
        </v-col>
        <v-col cols="3"
               class="pa-0"
               align="center" justify="center"
        >
          <v-img src="/nascente.jpg" style="height: 315px; width: 448px"></v-img>

          <v-img src="/header.jpg" style="height: calc(100vh - 315px); width: 448px">
            <v-overlay
              absolute
              opacity="0.8"
              color="accent"
            >
              <v-card tile class="pb-10 white--text shadow-0" elevation="0" color="transparent">
                <v-card-title style="width: 100%" class="justify-center text-h5">
                  Conheça o formato de <br/>NASCENTE PROTEGIDA
                </v-card-title>
                <v-card-text class="white--text text-subtitle-1">
                  is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's
                  standard dummy text ever since the 1500s, when an unknown printer took a galley of type and
                  scrambled
                  it to make a type specimen book. It has survived not only five centuries, but also the leap into
                </v-card-text>
              </v-card>


              <v-btn
                x-large
                width="90%"
                class="font-weight-bold font-italic"
                color="#1FCB42"
              >
                <span class="accent--text">
                  SAIBA MAIS SOBRE O PROJETO
                </span>
              </v-btn>

              <v-btn
                x-large
                width="90%"
                class="mt-4 font-weight-bold font-italic"
                color="#E99D45"
              >
                <span class="accent--text">
                  DÚVIDAS?
                </span>
                <span class="white--text">
                  FALE CONOSCO
                </span>
              </v-btn>
            </v-overlay>
          </v-img>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  layout: 'externo',
  name: "cadastro-dois"
}
</script>

<style scoped>
.v-text-field {
  margin: 0 !important;
  padding: 0 !important;
}

</style>
