<template>
  <div class="offer">
    <div class="container">
      <div class="offer-wrapper">
        <div class="fruit-offer">
          <div class="fruit-img-wrapper">
            <img src="@/assets/images/offer-img.png" alt="" />
            <div class="fruit-text">
              <p>Natural!!</p>
              <h5>
                Get Garden <br />
                Fresh Fruits
              </h5>
            </div>
          </div>
        </div>
        <div class="fruit-offer">
          <div class="sales-img-wrapper">
            <img src="@/assets/images/offer-img2.png" alt="" />
            <div class="fruit-text green">
              <p>Offer!!</p>
              <h5>
                Get 10% off <br />
                on Vegetables
              </h5>
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
.offer {
  padding: 50px 0;

  &-wrapper {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  .fruit-offer {
    position: relative;

    .fruit-text {
      position: absolute;
      top: 30%;
      left: 10%;

      p {
          font-family: Tail;
        font-size: 36px;
        color: #ffffff;
      }

      h5 {
          font-family: Robot;
        font-size: 40px;
        color: #ffffff;
      }
          &.green {
            p {
              color: #7eb693;
            }
    
            h5 {
              color: #274c5b;
            }
          }
    }
  }
}
</style>
