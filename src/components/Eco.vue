<template>
  <div class="eco">
    <div class="container">
      <div class="eco-wrapper">
        <div class="eco-img-wrapper">
          <img src="@/assets/images/eco-img.png" alt="" />
        </div>
        <div class="eco-infos">
          <div class="eco-info-titles">
            <p>Eco Friendly</p>
            <h3>
              From our Farm <br />
              to your Home.
            </h3>
          </div>
          <div class="content-wrapper">
            <div class="content-products">
              <h6>Choose Your Products</h6>
              <p>
                In our listing, we have several collections of organic products.
                This is the place where you need to choose the product you want.
              </p>
            </div>
            <div class="content-farmers">
              <h6>Farmers will produce it</h6>
              <p>
                The Product that you ordered will be verified that we have or
                not if have we will start to move on with the next step.
              </p>
            </div>
            <div class="content-delivery">
              <h6>We Can Delivery too</h6>
              <p>
                If you are not comfortable going to the nearby market place we
                also will deliver your product to your doorstep.
              </p>
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
.eco {
  display: flex;
  flex: 1;
  padding: 50px 0;
  
  &-wrapper {
    display: flex;
    justify-content: space-between;
  }

  &-infos {
    padding: 40px 0 40px 60px;
    width: 50%;
    height: 40%;
    transform: translate(-30%,  10%);
    position: relative;
    z-index: 111;
    background: #ffffff;
    border-radius: 20px 0 0 20px;
  }

  &-img-wrapper {
    position: relative;

    img {
      width: 100%;
      height: 100%;
      object-fit: cover;
    }
  }

  &-info-titles {
    display: flex;
    flex-direction: column;
    margin-bottom: 30px;

    p {
      font-family: Tail;
      font-size: 36px;
      line-height: 65px;
      color: #7eb693;
    }

    h3 {
      font-family: Robot;
      font-weight: 700;
      font-size: 44px;
      line-height: 58px;
      color: #274c5b;
    }
  }

  .content-wrapper {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    gap: 10px;

    h6 {
      font-family: Robot;
      font-weight: 700;
      font-size: 23px;
      line-height: 32px;
      color: #274c5b;
    }

    p {
      font-family: Robot;
      font-weight: 400;
      font-size: 18px;
      line-height: 32px;
      color: #525c60;
    }
  }
}
</style>
