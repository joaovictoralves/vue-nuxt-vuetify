<template>
  <div>
    <v-container>
      <v-card>
        <v-card-title>
          Cadastro de Propriedade Rural (CAR)
        </v-card-title>

        <v-card-subtitle>
          <div class="row">
            <div class="col-12">Número de registro no CAR:</div>
            <div class="col-12">Módulos fiscais:</div>
          </div>
        </v-card-subtitle>

        <v-card-text>
          <v-row>
            <v-col md="8" sm="12">
              <v-textarea
                solo
                rows="10"
                label="Aqui vai ficar o mapa"
              ></v-textarea>
            </v-col>
            <v-col md="4" sm="12">
              <v-textarea
                solo
                label="Aqui vai ficar o mapa"
              ></v-textarea>
            </v-col>
          </v-row>

          <v-row>
            <v-col md="12" sm="12">
              <v-textarea
                outlined
                label="Informações Gerais"
              ></v-textarea>
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
    </v-container>
  </div>
</template>

<script>
export default {
  name: "localizacao"
}
</script>

<style scoped>

</style>
