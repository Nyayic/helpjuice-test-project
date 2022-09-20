<!-- eslint-disable vue/multi-word-component-names -->
<template>
    <v-toolbar flat>
        <v-btn icon>
          <v-icon>mdi-chevron-double-right</v-icon>
        </v-btn>
        <v-btn icon>
          <v-icon>mdi-book-open-blank-variant</v-icon>
        </v-btn>

        <v-breadcrumbs :items="items" large></v-breadcrumbs>
  
        <v-spacer></v-spacer>
  
        <p>
        <v-btn icon>
          <v-icon>mdi-lock-open-outline</v-icon>
        </v-btn>
        Editing
        </p>
        <v-divider class="mx-1" vertical></v-divider>
        
        <p class="blue--text">
        Publishing Space
        <v-btn icon>
        <v-icon>mdi-chevron-down</v-icon>
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