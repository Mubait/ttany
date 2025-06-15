<template>
    <div class="main-block">
        <ProductFilter/>

        <div class="products-grid">
          <div class="products-grid-product" v-for="i in 12" :key="i">
            <div class="products-grid-product-img"></div>
            
            <div class="products-grid-product-labels">
              <p class="products-grid-product-brand-txt"> Бренд </p>
              <p class="products-grid-product-name-txt"> Полное название товара в несколько строк для вида с обрывом в конце. </p>
            </div>

            <div class="products-grid-product-price">
              <p class="products-grid-product-price-currentprice"> 5 990 ₽ </p>
              <p class="products-grid-product-price-oldprice"> 5 990 ₽ </p>
            </div>

            <div class="products-grid-product-buybtn" tabindex="0" @click ="buyBtnClick($event)">
              Купить
            </div>
          </div>
        </div>

    </div>

    
</template>

<script>
import ProductFilter from './ProductFilter.vue';

export default {
  name: 'MainBlock',
  components: {
    ProductFilter
  },
  methods: {
    buyBtnClick(event) {
      const buyBtn = event.target
      buyBtn.textContent = "Куплено!"
      buyBtn.style.border = "1px solid #D5D5D5"
      buyBtn.style.color = "#AAAAAA"
    }
  },
}
</script>