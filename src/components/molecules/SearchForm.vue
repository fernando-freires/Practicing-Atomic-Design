<template>
  <form class="search-form">
    <input type="search" placeholder="Buscar" />
    <button type="submit">
      <img src="@/assets/images/icons/search.svg" alt="Buscar" />
    </button>
  </form>
</template>

<style lang="scss" scoped>
.search-form {
  //estilização do formulario- posição na div
  position: relative;
  width: max-content;
  transition: transform 0.2s linear;
  //Transição ao passar o mouse por cima
  &:hover {
    transform: scale(1.1);
  }
  input {
    // estilização do input
    border: none;
    border-radius: 1rem;
    padding: 0.5rem 1rem;
    box-shadow: 0px 5px 5px rgba(#000000, 1);
    &::placeholder {
      color: #a9b0be;
    }
  }
  button {
    //deixar o botão bonito, definir tamanho, espaçamento e etc
    position: absolute;
    right: 3px;
    top: 50%;
    transform: translateY(-50%);
    width: 30px;
    height: 30px;
    background: #ff895f;
    border: none;
    border-radius: 5rem;
    //onde os itens ficam dentro do botão
    display: grid;
    justify-items: center;
    align-items: center;
  }
}
</style>
