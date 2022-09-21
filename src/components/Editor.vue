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
    <v-container >
        <v-row class="" justify="center" no-gutters>
            <v-col lg="8">
                <vue-editor v-model="content" :editor-toolbar="customToolbar"/>
                <Mentionable :keys="['/']" :items="items">
                    <textarea v-model="text" class="mention-item"/>
                </Mentionable>
            </v-col>
        </v-row>
    </v-container>
  </template>

<script>
import { VueEditor } from "vue2-editor";
import { Mentionable } from 'vue-mention';

export default {
    components: {
        VueEditor,
        Mentionable,
    },
    
    data () {
        return {
            content: "<h1>This is my header</h1>",
            customToolbar: [
                ["bold", "italic", "underline"],
            ],
            
            text: '',
            items: [
                {
                
                    value: 'Heading 1',
                    label: 'Heading !',
                },
                {
                    value: 'Expandable Heading 1',
                    label: 'Expandable Heading 1',
                },
            ],
        }
    }
}
</script>
