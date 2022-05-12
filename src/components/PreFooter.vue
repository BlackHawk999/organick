<template>
  <div class="pre-footer">
    <div class="container">
      <div class="pre-footer-wrapper">
        <div class="pre-footer-title">
          <h3>
            Subscribe our <br />
            Newsletter
          </h3>
        </div>
        <div class="pre-footer-email">
          <input type="email" placeholder="Enter your email address" />
          <button>Subscribe</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.pre-footer {
    padding-bottom: 50px;
    
  &-wrapper {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 100px 70px;
    background-image: url("@/assets/images/pre-footer-img.png");
    background-repeat: no-repeat;
    background-size: coverx;
    border-radius: 30px;
  }

  &-title {
    h3 {
      font-family: Robot;
      font-weight: 700;
      font-size: 50px;
      line-height: 60px;
      color: #ffffff;
    }
  }

  &-email {
    display: flex;
    align-items: center;
    gap: 20px;

    input {
      padding: 26px 50px 26px 30px;
      font-family: Robot;
      font-size: 18px;
      line-height: 29px;
      background: #ffffff;
      border: 1px solid #cccccc;
      border-radius: 16px;
      outline: none;
    }

    button {
      font-family: Robot;
      font-weight: 700;
      font-size: 18px;
      line-height: 29px;
      padding: 26px 36px;
      color: #ffffff;
      background: #274c5b;
      border: 1px solid #274c5b;
      border-radius: 16px;
      border: none;
      cursor: pointer;
      transition: 0.5s all;

      &:hover {
        color: #274c5b;
        background: #ffffff;
      }
    }
  }
}
</style>
