<!-- eslint-disable vue/multi-word-component-names -->
<!--template>
     <v-container >
        <v-row class="" justify="center" no-gutters>
            <v-col lg="8">
                <vue-editor v-model="content" :editor-toolbar="customToolbar"/>
            </v-col>
        </v-row>
    </v-container>
  </!--template>
  
   <script>
  import { VueEditor } from "vue2-editor";
  
  export default {
    components: { VueEditor },
  
    data: () => ({
        content: "<h1>This is my header</h1>",
        customToolbar: [
            ["bold", "italic", "underline"],
            
        ]
    })
  };
  </script> -->
  <template>
    <Mentionable
      :keys="['@']"
      :items="items"
      offset="6"
    >
      <textarea v-model="text"/>
    </Mentionable>
  </template>

<script>
import { Mentionable } from 'vue-mention'



export default {
    
  components: {
    Mentionable,
  },
  data () {
    return {
      text: '',
      items: [
        {
          value: 'cat',
          label: 'Mr Cat',
        },
        {
          value: 'dog',
          label: 'Mr Dog',
        },
      ],
    }
  },
}
</script>