<template>
  <v-app>
    <v-main>
      <Navbar />
      <TopHeader />
      <BottomHeader />
      <router-view></router-view>
    </v-main>
  </v-app>
</template>

<script>
import Navbar from '@/components/Navbar.vue'
import TopHeader from '@/components/TopHeader.vue'
import BottomHeader from '@/components/BottomHeader.vue'
export default {
  name: 'App',
    // register the components
  components: { Navbar, TopHeader, BottomHeader },

  data: () => ({
    //
  }),
};
</script>