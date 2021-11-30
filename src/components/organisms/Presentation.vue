<template>
  <div class="presentation">
    <SocialNetworks />

    <img
      class="presentation"
      src="@/assets/images/presentation.svg"
      alt="Apresentação"
    />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import { SocialNetworks } from '@/components/molecules'

export default defineComponent({
  components: { SocialNetworks }
})
</script>

<style lang="scss" scoped>
.presentation {
  //posição absolutas e fixas que movem o objeto. relative ok de se usar
  position: relative;
  display: grid;
  justify-content: center;
  .presentation {
    width: 80%;
    justify-self: center;
  }
  .social-networks {
    //posição das imagens/links das redes siciais
    position: absolute;
    left: 0;
    //Para centralizar
    top: 50%;
    transform: translateY(-50%);
  }
}
</style>
