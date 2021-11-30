<template>
  <a class="nav-item" :href="to">
    {{ text }}
  </a>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  props: {
    text: {
      //tipo
      type: String,
      required: true
    },
    to: {
      //para onde vai ao clicar
      type: String,
      required: true
    }
  }
})
</script>

<style lang="scss" scoped>
.nav-item {
  //estilização do link da barra de nav
  color: #293947;
  text-decoration: none;
  font-size: 1.3rem;
  transition: transform 0.2s linear;
  //Transição ao passar o mouse por cima
  &:hover {
    transform: scale(1.3);
  }
}
</style>
