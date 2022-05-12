<template>
  <div class="intro">
    <div class="container">
      <div class="intro-wrapper">
        <div class="intro-text">
          <p>Made with nature</p>
          <h1>
            Welcome to the <br />
            world of nature <br />and organic.
          </h1>
          <button>
            <span>Explore Now</span>
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
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.intro {
  width: 100%;
  height: 100vh;
  background-image: url(../assets/images/back-img.png);
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;

  &-wrapper {
    display: flex;
    justify-content: flex-start;
    align-items: center;
    min-height: 100vh;
  }

  &-text {
    width: 50%;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;

    p {
      font-family: Tail;
      font-size: 36px;
      margin-bottom: 14px;
      color: #7eb693;
    }

    h1 {
      font-family: Robot;
      font-size: 70px;
      font-weight: 700;
      line-height: 84px;
      margin-bottom: 30px;
      color: #274c5b;
    }

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
}
</style>
