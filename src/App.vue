<template>
  <HomeTemplate />
</template>

<script lang="ts">
import { defineComponent } from 'vue'
//importando o componente, que está exportado na index.ts
import { HomeTemplate } from '@/components/templates'

export default defineComponent({
  //declarando componente
  components: { HomeTemplate }
})
</script>
