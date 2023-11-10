<script setup>
</script>

<template>
  <main>
    <div class="produtos">
      <div class="produto">
        <div class="image-produto" style="background-image: url('https://fakestoreapi.com/img/81fPKd-2AYL._AC_SL1500_.jpg');"></div>
        <h4>Fjallraven - Foldsack No. 1 Backpack, Fits 15 Laptops</h4>
        <p class="preco">R$ 109.95</p>
        <button>Adicionar ao carrinho</button>
      </div>
      <div class="produto">
      <div class="image-produto" style="background-image: url('https://fakestoreapi.com/img/71-3HjGNDUL._AC_SY879._SX._UX._SY._UY_.jpg');"></div>
        <h4>Mens Casual Premium Slim Fit T-Shirts </h4>
        <p class="preco">R$ 22.30</p>
        <button>Adicionar ao carrinho</button>
      </div>
      <div class="produto">
      <div class="image-produto" style="background-image: url('https://fakestoreapi.com/img/71li-ujtlUL._AC_UX679_.jpg');"></div>
        <h4>Mens Cotton Jacket</h4>
        <p class="preco">R$ 55.99</p>
        <button>Adicionar ao carrinho</button>
      </div>

    </div>
  </main>
</template>

<style lang="scss">

.produtos {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  width: 100%;
  flex-direction: row;
  margin-top: 80px;
  text-align: center;

  .produto {
    flex: 0 0 30%;
    box-sizing: border-box;
    box-shadow: 0 4px 8px rgba(0,0,0,0.2);
    padding: 16px;
    margin: 8px;
    height: 360px;

    &.noCarrinho {
      border: 1px solid #007bff;
    }

    .image-produto {
      margin: 20px auto;
      width: 169px;
      height: 140px;
      background-size: contain;
      background-position: center;
      background-repeat: no-repeat;
    }

    h4 {
      margin: 22px auto;
      font-size: 12px;
      max-width: 80%;
    }

    .preco {
      font-size: 20px;
      font-weight: bold;
    }

    button {
      color: #fff;
      background-color: #007bff;
      border: 1px solid #007bff;
      border-radius: 100px;
      padding: 8px 16px;
      cursor: pointer;

      &:hover {
        opacity: 0.7;
      }

      &.remover {
        background-color: transparent;
        border: none;
        color: black;
        text-decoration: underline;
      }
    }

    @media only screen and (max-width: 769px) {
      flex: 0 0 40%;
    }
  
    @media only screen and (max-width: 640px) {
      flex: 0 0 90%;
    }
  }
}
</style>