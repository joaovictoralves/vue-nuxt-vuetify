<template>
  <v-app light>
    <v-main class="grey lighten-5 pa-0 ma-0">
      <v-container class="pa-0" style="width: 100vw;">
        <nuxt/>
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: 'mdi-apps',
          title: 'Welcome',
          to: '/'
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Inspire',
          to: '/inspire'
        },
        {
          icon: 'mdi-account-plus',
          title: 'Cadastro',
          to: '/cadastro'
        },
        {
          icon: 'mdi-account-plus',
          title: 'Cadastro 2',
          to: '/cadastro-dois'
        },
        {
          icon: 'mdi-compass',
          title: 'Localizacao',
          to: '/localizacao'
        },
        {
          icon: 'mdi-account-group',
          title: 'About',
          to: '/about'
        }
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'Vuetify.js'
    }
  }
}
</script>

<style>
.container {
  max-width: 98vw;
  padding: 0px;
}
</style>
