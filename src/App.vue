<template>
  <v-app>
    <v-main>
      <Navbar />
      <TopHeader />
      <BottomHeader />
      <Editor02/>
      <router-view></router-view>
    </v-main>
  </v-app>
</template>

<script>
  import Navbar from '@/components/Navbar.vue'
  import TopHeader from '@/components/TopHeader.vue'
  import BottomHeader from '@/components/BottomHeader.vue'
  import Editor02 from '@/components/Editor02.vue';
  
export default {
  name: 'App',
    // register the components
  components: { Navbar, TopHeader, BottomHeader, Editor02},
  data: () => ({
    //
  }),
};
</script>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Inter&display=swap');

  body, html{
    font-family: 'Inter', sans-serif;
  }
  .v-divider{
  max-height: 60% !important;
}

</style>
