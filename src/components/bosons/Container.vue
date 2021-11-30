<template>
  <div class="container">
    <slot />
  </div>
</template>

<style lang="scss" scoped>
.container {
  width: 85%;
  max-width: 1150px;
  // esse auto servirá para deixar o espaçamento igual de um lado e do outro
  margin: 0 auto;
}
</style>
