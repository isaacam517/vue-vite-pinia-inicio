<script setup>
</script>

<template>
  <div class="carrinho">
    <div class="itens">
      <div class="item">
        <div class="remover">Remover Produto</div>
        <div class="img-produto"><img src="https://fakestoreapi.com/img/71-3HjGNDUL._AC_SY879._SX._UX._SY._UY_.jpg" alt=""></div>
        <div class="descricao">Mens Casual Premium Slim Fit T-Shirts</div>
        <div class="preco">
          <span class="area-quantidade">
            <button disabled="">-</button>
            <span class="quantidade">1</span>
            <button >+</button>
          </span>
          <span class="total-item">R$ 22.30</span>
        </div>
      </div>
    </div>
    <div class="total-pedido">Total do pedido: R$ 22.30</div>
  </div>
</template>

<style lang="scss">

.carrinho {
  padding: 60px 0;

  .itens {
    max-width: 800px;
    margin: auto;

    .item {
      display: flex;
      justify-content: space-between;
      padding: 40px 0;
      border-bottom: 1px solid lightgrey;
      position: relative;

      .remover {
        position: absolute;
        top: 8px;
        right: 0;
        font-size: 11px;
        text-decoration: underline;
        cursor: pointer;
      }
      
      .img-produto {
        img {
          max-width: 80px;
        }
      }
      
      .title {
        padding-left: 30px;
        box-sizing: border-box;
        max-width: 50%;
      }
      
      .preco {
        .area-quantidade {
          margin: 8px auto;
          height: 14px;
        
          button {
            width: 16px;
            height: 16px;
            display: inline-flex;
            justify-content: center;
            align-items: center;
            cursor: pointer;
          }

          .quantidade {
            margin: 0 4px;
          }
        
        }

        .total-item {
          font-size: 16px;
          margin-left: 8px;
          text-align: right;
          vertical-align: middle;
        }
      }
    }
  }
  .total-pedido {
    font-size: 24px;
    font-weight: bold;
    text-align: right;
    margin-top: 8px;
    margin-right: 50px;
  }
}

</style>
