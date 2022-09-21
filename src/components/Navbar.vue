<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <v-toolbar flat class="my-0 text-sm-body-2">
    <v-btn icon>
      <v-icon small>mdi-chevron-double-right</v-icon>
    </v-btn>
    <v-btn icon>
      <v-icon small>mdi-book-open-blank-variant</v-icon>
    </v-btn>

    <v-breadcrumbs :items="items"></v-breadcrumbs>
  
    <v-spacer></v-spacer>
  
    <p class="text--disabled">
      <v-btn icon>
        <v-icon small>mdi-lock-open-outline</v-icon>
      </v-btn>
      Editing
    </p>
    <v-divider class="mx-4 divider" inset vertical  width="100"></v-divider>
        
    <p class="publish text-sm-body-2">
      Publish Space
      <v-btn icon>
        <v-icon small>mdi-chevron-down</v-icon>
      </v-btn>
    </p>
  </v-toolbar>
    
</template>


<script>
  export default {
    data: () => ({
      items: [
        {
          text: 'Main',
          disabled: true,
          href: 'main',
        },
        {
          text: 'Getting Started',
          disabled: true,
          href: 'getting_started',
        },
        {
          text: 'Front-end developer test proje...',
          disabled: true,
          href: 'front-end_test project',
        },
      ],
    }),
  }
</script>
<style>
  .publish{
    color: #058DDA !important;
    font-weight: 400;
  }
 
 
</style>