<template>
  <div class="services">
    <Service
      title="Front End"
      description="Lorem ipsum dolor sit, amet consectetur adipisicing elit. Blanditiis modi, pariatur aspernatur corrupti maxime iure accusamus reiciendis nihil, debitis dolorem beatae fuga et repudiandae! Assumenda facilis temporibus debitis iure in."
    />

    <Service
      title="Back End"
      description="Lorem ipsum dolor sit, amet consectetur adipisicing elit. Blanditiis modi, pariatur aspernatur corrupti maxime iure accusamus reiciendis nihil, debitis dolorem beatae fuga et repudiandae! Assumenda facilis temporibus debitis iure in."
    />

    <Service
      title="Manutenção"
      description="Lorem ipsum dolor sit, amet consectetur adipisicing elit. Blanditiis modi, pariatur aspernatur corrupti maxime iure accusamus reiciendis nihil, debitis dolorem beatae fuga et repudiandae! Assumenda facilis temporibus debitis iure in."
    />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import { Service } from '@/components/molecules'

export default defineComponent({
  components: { Service }
})
</script>

<style lang="scss" scoped>
.services {
  display: grid;
  //Criar as 3 colunas onde cada service será colocado
  grid-template-columns: repeat(3, 1fr);
  grid-gap: 5rem;
}
</style>
