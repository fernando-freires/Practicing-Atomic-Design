<template>
  <div class="social-networks">
    <SocialLink
      name="GitHub"
      to="https://github.com/fernando-freires"
      icon="github.svg"
    />

    <SocialLink
      name="Twitter"
      to="https://Twitter.com/fernando-freires"
      icon="twitter.svg"
    />

    <SocialLink
      name="Facebook"
      to="https://Facebook.com/fernando-freires"
      icon="facebook.svg"
    />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
//importando o componente, que está exportado na index.ts
import { SocialLink } from '@/components/atoms'

export default defineComponent({
  //declarando componente
  components: { SocialLink }
})
</script>

<style lang="scss" scoped>
.social-networks {
  display: grid;
  grid-gap: 1rem;
}
</style>
