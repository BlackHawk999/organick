<template>
  <div class="product-item">
    <div class="product-img-wrapper">
      <p class="product-type-name">{{ kind }}</p>
      <img :src="imgUrl" />
    </div>
    <div class="product-name-wrapper">
      <p>{{ title }}</p>
    </div>
    <div class="product-infos">
      <h6 class="product-price">{{ price }} $</h6>
      <i class="product-rate">
        <svg
          v-for="item in 5"
          :key="item"
          width="15"
          height="14"
          viewBox="0 0 15 14"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            d="M6.82942 0.781287C7.13702 -0.122413 8.41509 -0.122403 8.72279 0.781287L9.70629 3.67075C9.84419 4.07602 10.2248 4.34853 10.6529 4.34853H13.7331C14.7131 4.34853 15.1083 5.61178 14.303 6.17025L11.8923 7.84218C11.5254 8.09662 11.3717 8.56342 11.5155 8.98612L12.455 11.7462C12.7658 12.6594 11.7311 13.4399 10.9385 12.8901L8.34599 11.0922C8.00319 10.8544 7.54893 10.8544 7.20619 11.0922L4.61371 12.8901C3.82104 13.4399 2.78632 12.6594 3.09715 11.7462L4.03664 8.98612C4.18051 8.56342 4.02675 8.09662 3.65987 7.84218L1.24913 6.17025C0.443886 5.61178 0.839076 4.34853 1.81902 4.34853H4.89923C5.32733 4.34853 5.70795 4.07602 5.8459 3.67075L6.82942 0.781287Z"
            fill="#FFA858"
          />
        </svg>
      </i>
    </div>
  </div>
</template>

<script>
export default {
  name: "product-item",
  props: {
    kind: {
      type: String,
    },
    imgUrl: {
      type: String,
    },
    title: {
      type: String,
    },
    price: {
      type: Number,
    },
  },
};
</script>

<style lang="scss" scoped>
.product {
  &-item {
    padding: 30px;
    background: #f9f8f8;
    border-radius: 30px;
    overflow: hidden;
    transition: 0.4s all;
    cursor: pointer;

    &:hover {
      transform: scale(1.1);
    }
  }
  &-img-wrapper {
    position: relative;
  }
  &-type-name {
    position: absolute;
    padding: 2px;
    font-family: Robot;
    font-weight: 700;
    font-size: 15px;
    line-height: 27px;
    color: #ffffff;
    background: #274c5b;
    border-radius: 8px;
  }
  &-name-wrapper {
    border-bottom: 1px solid #d4d4d4;
    padding-bottom: 10px;
    margin-bottom: 10px;

    p {
      font-family: Robot;
      font-size: 22px;
      font-weight: 400;
      line-height: 35px;
      color: #274c5b;
    }
  }
  &-infos {
    display: flex;
    align-items: center;
    justify-content: space-between;

    h6 {
      font-family: Robot;
      font-weight: 700;
      font-size: 18px;
      line-height: 32px;
      color: #274c5b;
    }
  }
}
</style>
