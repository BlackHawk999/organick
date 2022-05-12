<template>
  <div class="products">
    <div class="container">
      <div class="products-wrapper">
        <div class="products-title">
          <p>Organic</p>
          <h3>Our Products</h3>
        </div>
        <div class="products-list">
          <Product-item
            v-for="(p, i) in products"
            :key="i"
            :kind="p.kind"
            :title="p.title"
            :img-url="p.imgUrl"
            :price="p.price"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import ProductItem from "@/components/products/ProductItem.vue";

export default {
  name: "Products",
  components: { ProductItem },
  data() {
    return {
      products: [
        {
          kind: "vegetable",
          title: "Calabrese Broccoli",
          imgUrl: require("@/assets/images/product-brookli.png"),
          price: 25.0,
        },
        {
          kind: "vegetable",
          title: "Calabrese Broccoli",
          imgUrl: require("@/assets/images/product-corn.png"),
          price: 23.0,
        },
        {
          kind: "mill",
          title: "Calabrese Broccoli",
          imgUrl: require("@/assets/images/product-img.png"),
          price: 22.0,
        },
        {
          kind: "vegetable",
          title: "Calabrese Broccoli",
          imgUrl: require("@/assets/images/product-almon.png"),
          price: 17.0,
        },
        {
          kind: "fru",
          title: "Calabrese Broccoli",
          imgUrl: require("@/assets/images/product-tomato.png"),
          price: 12.0,
        },
        {
          kind: "fru",
          title: "Calabrese Broccoli",
          imgUrl: require("@/assets/images/product-nuts.png"),
          price: 15.0,
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.products {
  padding: 50px 0;
  &-title {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-bottom: 45px;

    p {
      font-family: Tail;
      font-size: 36px;
      line-height: 65px;
      color: #7eb693;
      text-transform: uppercase;
    }

    h3 {
      font-family: Robot;
      font-weight: 700;
      font-size: 45px;
      line-height: 58px;
      text-transform: uppercase;
    }
  }
  &-list {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    column-gap: 30px;
    row-gap: 30px;
  }
}
</style>
