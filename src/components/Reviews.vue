<template>
  <div class="reviews">
    <div class="container">
      <div class="reviews-wrapper">
        <div class="reviewer-wrapper">
          <div class="reviews-title">
            <p>Testimonial</p>
            <h3>What Our Customer Saying?</h3>
          </div>
          <div class="reviwer-infos">
            <div class="reviewer-img-wrapper">
              <img src="@/assets/images/woman.jpg" alt="" />
            </div>
            <i class="review-rate">
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
          <div class="reviewer-texts">
            <p class="content">
              The quality of organic produce is extremely high, the service is
              second to none and the taste of the food <br />
              takes me back to my childhood when we were growing our own.
            </p>
            <h6 class="reviewer-name">Sara Taylor</h6>
            <p class="content type">Consumer</p>
          </div>
        </div>
        <div class="review-stats">
          <div class="statics">
            <h6>100%</h6>
            <p>organic</p>
          </div>
          <div class="statics">
            <h6>285</h6>
            <p>Active Product</p>
          </div>
          <div class="statics">
            <h6>385+</h6>
            <p>Organic Orchads</p>
          </div>
          <div class="statics">
            <h6>25+</h6>
            <p>Years of Farming</p>
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
.reviews {
  padding: 50px 0;
  background-image: url("@/assets/images/review-back.png");
  background-repeat: no-repeat;
  background-size: cover;

  &-wrapper {
    display: flex;
    flex-direction: column;
  }

  .reviewer-wrapper {
    padding-bottom: 35px;
    border-bottom: 3px solid #e0e0e0;
  }

  &-title {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-bottom: 60px;

    p {
      font-family: Tail;
      font-size: 36px;
      line-height: 65px;
      color: #7eb693;
      text-transform: uppercase;
    }

    h3 {
      font-family: Robot;
      font-size: 45px;
      line-height: 58px;
      color: #274c5b;
      text-transform: uppercase;
    }
  }

  .reviwer-infos {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 20px;
    margin-bottom: 35px;
  }

  .reviewer-img-wrapper {
    width: 115px;
    height: 115px;
    border-radius: 50%;
    overflow: hidden;

    img {
      width: 100%;
      height: 100%;
      object-fit: cover;
    }
  }

  .reviewer-texts {
    display: flex;
    flex-direction: column;
    align-items: center;

    .content {
      font-family: Robot;
      font-size: 18px;
      line-height: 32px;
      color: #525c60;
      text-align: center;
      margin-bottom: 25px;

      &.type {
        font-size: 14px;
      }
    }

    .reviewer-name {
      font-family: Robot;
      font-size: 26px;
      font-weight: 700;
      line-height: 34px;
      color: #274c5b;
    }
  }

  .review-stats {
    display: flex;
    align-items: center;
    justify-content: center;
    padding-top: 50px;
    gap: 35px;
  }

  .statics {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    width: 240px;
    height: 240px;
    background: #f1f1f1;
    border: 6px solid #7eb693;
    border-radius: 50%;

    h6 {
      font-family: Robot;
      font-weight: 700;
      font-size: 42px;
      line-height: 55px;
      color: #274c5b;
    }

    p {
      font-family: Robot;
      font-weight: 700;
      font-size: 18px;
      line-height: 32px;
      color: #274c5b;
    }
  }
}
</style>
