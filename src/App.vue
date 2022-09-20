<template>
  <v-app>
    <v-main>
      <Navbar />
      <Header />
      <router-view></router-view>
    </v-main>
  </v-app>
</template>

<script>
import Navbar from '@/components/Navbar.vue'
import Header from '@/components/Header.vue'
export default {
  name: 'App',
    // register the components
  components: { Navbar, Header },

  data: () => ({
    //
  }),
};
</script>