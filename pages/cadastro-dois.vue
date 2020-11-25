<template>
  <div>
    <v-container>
      <v-card>
        <v-card-title>
          Cadastro para acesso ao Portal
        </v-card-title>
        <v-card-text>
          <v-text-field
            label="CPF"
            outlined
            background-color="#FBFEFF"
          ></v-text-field>

          <v-text-field
            label="Nome"
            outlined
            background-color="#FBFEFF"
          ></v-text-field>

          <v-text-field
            label="CEP"
            outlined
            background-color="#FBFEFF"
          ></v-text-field>

          <v-select
            :items="['GO', 'TO']"
            label="Estado"
            outlined
            background-color="#FBFEFF"
          ></v-select>

          <v-text-field
            label="Cidade"
            outlined
            background-color="#FBFEFF"
          ></v-text-field>

          <v-text-field
            label="Bairro"
            outlined
            background-color="#FBFEFF"
          ></v-text-field>

          <v-text-field
            label="Rua/Avenida"
            outlined
            background-color="#FBFEFF"
          ></v-text-field>

          <v-text-field
            label="Número"
            outlined
            background-color="#FBFEFF"
          ></v-text-field>


          <v-text-field
            label="Quadra"
            outlined
            background-color="#FBFEFF"
          ></v-text-field>

          <v-text-field
            label="Lote"
            outlined
            background-color="#FBFEFF"
          ></v-text-field>

          <v-row>
            <v-col md="12" sm="12">
              <v-text-field
                label="Complemento"
                outlined
                background-color="#FBFEFF"
              ></v-text-field>
            </v-col>
          </v-row>

          <v-row>
            <v-col lg="3" md="6" sm="12">
              <v-text-field
                label="Telefone"
                outlined
                background-color="#FBFEFF"
              ></v-text-field>
            </v-col>
            <v-col lg="3" md="6" sm="12">
              <v-text-field
                label="Celular"
                outlined
                background-color="#FBFEFF"
              ></v-text-field>
            </v-col>
          </v-row>

          <v-row>
            <v-col lg="3" md="6" sm="12">
              <v-text-field
                label="E-mail"
                outlined
                background-color="#FBFEFF"
              ></v-text-field>
            </v-col>
            <v-col lg="3" md="6" sm="12">
              <v-text-field
                label="Confirmar E-mail"
                outlined
                background-color="#FBFEFF"
              ></v-text-field>
            </v-col>
          </v-row>

          <v-row>
            <v-col lg="3" md="6" sm="12">
              <v-text-field
                label="Senha"
                outlined
                background-color="#FBFEFF"
              ></v-text-field>
            </v-col>
            <v-col lg="3" md="6" sm="12">
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
    </v-container>
  </div>
</template>

<script>
export default {
  name: "cadastro"
}
</script>

<style scoped>

</style>
