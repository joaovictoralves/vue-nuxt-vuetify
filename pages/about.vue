<template>
  <div>
    <v-container style="height: 100vh">
      <!--      <v-row style="height: 100vh" justify="start" align="center">-->
      <v-row style="height: 100vh" justify="start">
        <v-col md="8" sm="12">
          <v-card>
            <v-card-title>
              Sobre nós
            </v-card-title>
            <v-card-text>
              Hello World!
            </v-card-text>
          </v-card>
        </v-col>
        <v-col md="4" sm="12">
          <v-scroll-y-reverse-transition>
            <v-card>
              <v-card-title>
                Sobre nós
              </v-card-title>
              <v-card-text>
                Hello World!
              </v-card-text>
            </v-card>
          </v-scroll-y-reverse-transition>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  name: "about"
}
</script>

<style scoped>

</style>
