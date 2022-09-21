<!-- eslint-disable vue/multi-word-component-names -->
<template>
    <v-container >
        <v-row class="" justify="center" no-gutters>
            <v-col lg="8">
                <ckeditor :editor="editor" v-model="editorData" :config="editorConfig"></ckeditor>
            </v-col>
        </v-row>
    </v-container>
</template>

<script>
import ClassicEditor from '@ckeditor/ckeditor5-build-classic';

    export default {
        name: 'app',
        data() {
            return {
                editor: ClassicEditor, 
                editorData: '',
                editorConfig: {
                    // The configuration of the editor.
                    toolbar: [ 'heading 1' ],
                   
                },
               
            };
        }
    }
</script>