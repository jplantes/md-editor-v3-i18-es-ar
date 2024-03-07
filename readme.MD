# Paquete i18n Español para md-editor-v3

Como utilzar el paquete

1.- Instalar el paquete md-editor-v3

```sh
npm i md-editor-v3
```

2.- Instalar el paquete de idioma

```sh
npm i md-editor-v3-i18-es-ar
```

3.- Como utilizarlo

```javascript
<script setup lang="ts">
import { ref } from 'vue'
import { MdEditor, config } from 'md-editor-v3'
import 'md-editor-v3/lib/style.css'
import ES_AR from '@/utilities/i18n/es_AR'

const text = ref('# ¿De que vas a hablar hoy?')

config({
  editorConfig: {
    languageUserDefined: {
      'es_AR': ES_AR
    }
  }
})

</script>

<template>
  <MdEditor v-model="text" language="es_AR" />
</template>
```
