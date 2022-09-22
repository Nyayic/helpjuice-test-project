<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <v-container >
    <v-row  justify="center" no-gutters>
      <v-col lg="8">
        <v-card class="mx-auto card"  flat outlined >
          <v-app-bar dense flat>
            <v-btn icon class="mx-0">
              <v-icon small>mdi-format-paragraph</v-icon>
            </v-btn>
            <v-divider vertical inset></v-divider>
            <v-btn icon>
                <v-icon small>mdi-clock-outline</v-icon> 
            </v-btn> 
            0 Mins
        
            <v-divider vertical inset class="mx-2"></v-divider>
           
            <v-avatar size="28" class="mx-2">
              <img src="../assets/avatar.png" alt="avatar">
            </v-avatar>
        
            <v-divider inset class="mx-2" vertical></v-divider>
        
            <v-btn icon>
                <v-icon small>mdi-arrow-bottom-left-thin</v-icon> 
            </v-btn> 0
        
            <v-spacer></v-spacer>
  
            <v-btn icon class="mx-2">
              <v-icon small>mdi-checkbox-marked-circle-outline</v-icon>
              <v-icon small>mdi-weather-cloudy</v-icon>
              <v-icon small>mdi-dots-vertical</v-icon>
            </v-btn>
  
          </v-app-bar>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>
<style>
  .theme--light.v-app-bar.v-toolbar.v-sheet {
	background-color: #fff !important;
}
.v-icon.notranslate.mdi.mdi-format-paragraph.theme--light {
	background: #d9f9e6;
	border-radius: 4px;
}

</style>