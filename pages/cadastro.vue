<template>
  <div
    class="primary"
  >
    <v-container class="pt-0">
      <v-row class="pt-0">
        <v-col cols="12" class="pa-0">
          <v-img src="/header.jpg" style="height: 400px">
            <v-overlay
              absolute
              color="#499A8C"
            >
              <v-container class="" style="width: calc(100vw - 300px)">
                <v-row>
                  <v-col cols="4" align="center" justify="center">
                    <img src="/logo.svg" style="height: 132px; width: 162px"/>
                  </v-col>
                  <v-col cols="8" align="end">
                      <span class="text-h4">
                        Projeto de Recuperação das Nascentes
                      </span>
                    <br/>
                    <span class="text-h6">
                        Bacias do Rio Meia Ponte e Ribeirão Piancó
                      </span>
                  </v-col>
                </v-row>
              </v-container>
            </v-overlay>
          </v-img>
        </v-col>
      </v-row>

      <v-row class="pr-6">
        <v-col cols="8" class="pl-10 pr-6">
          <v-card style="margin-top: -40px">
            <v-card-title>
              Cadastro para acesso ao Portal
            </v-card-title>
            <v-card-text>
              <v-row>
                <v-col lg="3" md="6" sm="12" class="pb-0">
                  <v-text-field
                    label="CPF"
                    outlined
                    background-color="#FBFEFF"
                    :rules="[ val => val && val.length <12  || 'CPF inválido!']"
                  ></v-text-field>
                </v-col>
                <v-col lg="9" md="6" sm="12" class="pb-0">
                  <v-text-field
                    label="Nome"
                    outlined
                    background-color="#FBFEFF"
                  ></v-text-field>
                </v-col>
              </v-row>

              <v-row>
                <v-col lg="3" md="6" sm="12" class="pt-0 pb-0">
                  <v-text-field
                    label="CEP"
                    outlined
                    background-color="#FBFEFF"
                  ></v-text-field>
                </v-col>
                <v-col md="3" sm="12" class="pt-0 pb-0">
                  <v-select
                    :items="['GO', 'TO']"
                    label="Estado"
                    outlined
                    background-color="#FBFEFF"
                  ></v-select>
                </v-col>
                <v-col md="6" sm="12" class="pt-0 pb-0">
                  <v-text-field
                    label="Cidade"
                    outlined
                    background-color="#FBFEFF"
                  ></v-text-field>
                </v-col>
              </v-row>

              <v-row>
                <v-col md="6" sm="12" class="pt-0 pb-0">
                  <v-text-field
                    label="Bairro"
                    outlined
                    background-color="#FBFEFF"
                  ></v-text-field>
                </v-col>
                <v-col md="6" sm="12" class="pt-0 pb-0">
                  <v-text-field
                    label="Rua/Avenida"
                    outlined
                    background-color="#FBFEFF"
                  ></v-text-field>
                </v-col>
              </v-row>

              <v-row>
                <v-col lg="3" md="6" sm="12" class="pt-0 pb-0">
                  <v-text-field
                    label="Número"
                    outlined
                    background-color="#FBFEFF"
                  ></v-text-field>
                </v-col>
                <v-col lg="3" md="6" sm="12" class="pt-0 pb-0">
                  <v-text-field
                    label="Quadra"
                    outlined
                    background-color="#FBFEFF"
                  ></v-text-field>
                </v-col>
                <v-col lg="6" md="6" sm="12" class="pt-0 pb-0">
                  <v-text-field
                    label="Lote"
                    outlined
                    background-color="#FBFEFF"
                  ></v-text-field>
                </v-col>
              </v-row>

              <v-row>
                <v-col md="12" sm="12" class="pt-0 pb-0">
                  <v-text-field
                    label="Complemento"
                    outlined
                    background-color="#FBFEFF"
                  ></v-text-field>
                </v-col>
              </v-row>

              <v-row>
                <v-col lg="3" md="6" sm="12" class="pt-0 pb-0">
                  <v-text-field
                    label="Telefone"
                    outlined
                    background-color="#FBFEFF"
                  ></v-text-field>
                </v-col>
                <v-col lg="3" md="6" sm="12" class="pt-0 pb-0">
                  <v-text-field
                    label="Celular"
                    outlined
                    background-color="#FBFEFF"
                  ></v-text-field>
                </v-col>
              </v-row>

              <v-row>
                <v-col lg="6" md="6" sm="12" class="pt-0 pb-0">
                  <v-text-field
                    label="E-mail"
                    outlined
                    background-color="#FBFEFF"
                  ></v-text-field>
                </v-col>
                <v-col lg="6" md="6" sm="12" class="pt-0 pb-0">
                  <v-text-field
                    label="Confirmar E-mail"
                    outlined
                    background-color="#FBFEFF"
                  ></v-text-field>
                </v-col>
              </v-row>

              <v-row>
                <v-col lg="6" md="6" sm="12" class="pt-0 pb-0">
                  <v-text-field
                    label="Senha"
                    outlined
                    background-color="#FBFEFF"
                  ></v-text-field>
                </v-col>
                <v-col lg="6" md="6" sm="12" class="pt-0 pb-0">
                  <v-text-field
                    label="Confirmar Senha"
                    outlined
                    background-color="#FBFEFF"
                  ></v-text-field>
                </v-col>
              </v-row>

              <v-row>
                <v-col style="text-align: center">
                  <v-btn
                    class="mr-4"
                    depressed
                    color="primary"
                  >
                    Confirmar
                  </v-btn>

                  <v-btn
                    class="ml-4"
                    depressed
                    color="error"
                  >
                    Cancelar
                  </v-btn>
                </v-col>
              </v-row>

            </v-card-text>
          </v-card>
        </v-col>
        <v-col cols="4"
               class="pl-6 pr-6 accent"
        >
          <v-img src="/nascente.jpg" style="width: 100%;"></v-img>

          <v-card shaped class="ml-4 mr-4 white--text" style="margin-top: -15px" color="#19AA75">
            <v-card-title style="width: 100%" class="justify-center text-h5">
              Conheça o formato de <br/>NASCENTE PROTEGIDA
            </v-card-title>
            <v-card-text class="white--text">
              is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's
              standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled
              it to make a type specimen book. It has survived not only five centuries, but also the leap into
            </v-card-text>
          </v-card>

          <v-card
            align="center"
            style="cursor: pointer"
            v-ripple
            class="mt-4 col-12 accent--text font-weight-bold font-italic"
            color="#1FCB42"
          >
            SAIBA MAIS SOBRE O PROJETO
          </v-card>

          <v-card
            align="center"
            style="cursor: pointer"
            class="mt-4 col-12 font-weight-bold font-italic"
            v-ripple
            color="#E99D45"
          >
            <span class="accent--text">
              DÚVIDAS?
            </span>
            <span class="white--text">
              FALE CONOSCO
            </span>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  name: "cadastro"
}
</script>

<style scoped>
.v-text-field {
  margin: 0 !important;
  padding: 0 !important;
}

</style>
