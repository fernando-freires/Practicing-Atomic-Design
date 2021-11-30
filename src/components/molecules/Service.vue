<template>
  <div class="service">
    <h2 class="title">{{ title }}</h2>
    <p class="description">{{ description }}</p>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  props: {
    //Definir os parametros da molecula
    title: { type: String, required: true },
    description: { type: String, required: true }
  }
})
</script>

<style lang="scss" scoped>
.service {
  .title {
    color: #935e92;
    font-weight: bold;
    margin-bottom: 0.7rem;
  }
  .description {
    color: #293947;
    line-height: 1.5;
  }
}
</style>
