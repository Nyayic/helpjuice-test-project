<template>
  <v-app>
    <v-main>
      <Navbar />
      <TopHeader />
      <BottomHeader />
      <Editor/>
      <router-view></router-view>
    </v-main>
  </v-app>
</template>

<script>
 

import Navbar from '@/components/Navbar.vue'
import TopHeader from '@/components/TopHeader.vue'
import BottomHeader from '@/components/BottomHeader.vue'
import Editor from '@/components/Editor.vue'

export default {
  name: 'App',
    // register the components
  components: { Navbar, TopHeader, BottomHeader, Editor },
  

  data: () => ({
    //
  }),
};
</script>