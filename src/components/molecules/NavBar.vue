<template>
  <nav class="nav-bar">
    <nav-item text="Serviços" to="/services" />
    <nav-item text="Sobre mim" to="/about" />
    <nav-item text="Cases" to="/home" />
    <nav-item text="Contatos" to="/contacts" />
  </nav>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
//importando componente atom para gerar uma molecula
import { NavItem } from '@/components/atoms'

export default defineComponent({
  components: { NavItem }
})
</script>

<style lang="scss" scoped>
.nav-bar {
  //estilização dos componentes da barra de navegação que ficarão dentro da div do app
  width: max-content;
  display: grid;
  grid-auto-flow: column;
  grid-gap: 2.5rem;
}
</style>
