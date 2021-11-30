<template>
  <a class="social-link" :href="to" target="_blank">
    <img :src="iconPath" :alt="name" />
    <!--em src ja há o caminho para nao ter que ficar repetindo no template de app. o caminho está definido em computed-->
  </a>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  props: {
    // Propriedades do que será inserido nos icones das redes sociais
    name: { name: String, required: true },
    icon: { name: String, required: true },
    to: { name: String, required: true }
  },
  computed: {
    iconPath() {
      return require(`@/assets/images/icons/${this.icon}`)
    }
  }
})
</script>

<style lang="scss" scoped>
.social-link {
  // estilização do link para as redes sociais
  background-color: #ff895f;
  width: 47px;
  height: 47px;
  border-radius: 5rem;
  // organização dos itens
  display: grid;
  justify-items: center;
  align-items: center;
  transition: transform 0.2s linear;
  //Transição ao passar o mouse por cima
  &:hover {
    transform: scale(1.3);
  }
  img {
    // estilizar a imagem
    width: 23px;
    height: 23px;
  }
}
</style>
