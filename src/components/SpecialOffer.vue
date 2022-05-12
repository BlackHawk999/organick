<template>
  <div class="special-offer">
    <div class="container">
      <div class="special-offer-wrapper">
        <div class="special-offer-header">
          <div class="special-offer-titles">
            <p>Offer Products</p>
            <h3>We Offer Organic for You</h3>
          </div>
          <div class="view-all-offer">
            <button>
              <span>View All Offer</span>
              <i class="icon-wrapper">
                <svg
                  width="17"
                  height="13"
                  viewBox="0 0 17 13"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M15.0384 6.50003H1M9.07688 1L16 6.50003L9.07688 12V1Z"
                    stroke="white"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                </svg>
              </i>
            </button>
          </div>
        </div>
        <div class="special-products">
          <product-item
            v-for="(p, i) in offerproducts"
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
  components: { ProductItem },

  data() {
    return {
      offerproducts: [
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
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.special-offer {
  padding: 70px 0;
  background: #274c5b;

  .view-all-offer {
    button {
      padding: 25px 25px 25px 30px;
      background: #efd372;
      border: 1px solid #efd372;
      border-radius: 16px;
      cursor: pointer;

      span {
        font-family: Robot;
        font-size: 19px;
        margin-right: 10px;
      }

      .icon-wrapper {
        padding: 12px 10px 10px 10px;
        background: #335b6b;
        border-radius: 50%;
      }
    }
  }

  .special {
    &-offer-header {
      display: flex;
      align-items: center;
      justify-content: space-between;
    }

    &-offer-titles {
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      margin-bottom: 50px;

      p {
        font-family: Tail;
        font-size: 36px;
        line-height: 65px;
        color: #7eb693;
      }

      h3 {
        font-family: Robot;
        font-weight: 700;
        font-size: 45px;
        line-height: 58px;
        color: #ffffff;
      }
    }

    &-products {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      column-gap: 30px;
    }
  }
}
</style>
