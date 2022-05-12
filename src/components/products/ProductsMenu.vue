<template>
  <div class="products-menu">
    <div class="container">
      <div class="products-menu-wrapper">
        <div class="products-item">
          <div class="products-img-wrapper">
            <img src="@/assets/images/menu-img.png" alt="" />
            <div class="product-menu-btn">
              <button>Fruit Juice</button>
            </div>
          </div>
          <div class="products-img-wrapper">
            <img src="@/assets/images/menu-green-img.png" alt="" />
            <div class="product-menu-btn">
              <button>Organic Food</button>
            </div>
          </div>
          <div class="products-img-wrapper">
            <img src="@/assets/images/menu-brown-img.png" alt="" />
            <div class="product-menu-btn">
              <button>Nuts Cookies</button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.products {
  &-menu {
    padding: 100px 0;
    background: #eff6f1;
  }
  &-item {
    display: flex;
    align-items: center;
    gap: 40px;
  }
  &-img-wrapper {
    position: relative;

    &:hover {
      img {
        filter: blur(3px);
        -webkit-filter: blur(3px);
      }

      .product-menu-btn {
        button {
          opacity: 1;
          filter: none;
          transform: scale(1.2);
        }
      }
    }

    .product-menu-btn {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);

      button {
        padding: 30px 80px;
        font-family: Robot;
        font-weight: 700;
        font-size: 24px;
        line-height: 35px;
        border-radius: 20px;
        border: none;
        white-space: nowrap;
        transition: 00.4s all;
        cursor: pointer;
        color: #274c5b;
      }
    }
  }
}
</style>
