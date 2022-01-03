<template>
  <div class="about">
    <div class="container">
      <div class="about-text">
        <div class="title">ABOUT US</div>

        <p>
          The occupational traffic permit is one of the most important things in the company when carrying out freight transport.  In fact, it is a prerequisite for doing business traffic at all. 
        </p>

        <div class="how-to">
          How do you do when you need to obtain a commercial traffic permit for freight transport to your business?
        </div>
      </div>

      <div id="instructor">
        <img src="@/assets/Illustration.svg"/>
      </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
  .about {
    padding: 100px 0;
    width: 100%;

    .container {
      position: relative;

      display: flex;
      flex-wrap: wrap;

      > div {
        flex-basis: 50%;
      }
    }

    &-text {
      .title {
        color: #EE4D47;
        font-weight: 700;
        font-size: 24px;
        line-height: 40px;

        padding: 20px 0;
      }

      p {
        width: 470px;
        font-weight: 300;
        font-size: 18px;
        line-height: 40px;
      }

      .how-to {
        margin-top: 80px;

        font-weight: 500;
        font-size: 24px;
        line-height: 36px;
        color: #402B2B;

        background: #FCDDD4;
        padding: 30px 55px;
        border-left: #EE4D47 solid 10px;

      }
    }

    #instructor {
      position: absolute;
      right: 0;
      opacity: 0;

      &.animate {
        opacity: 1;
        animation-name: instructor-enter;
        animation-duration: 1.5s; 
      }      
    }
  }

  @keyframes instructor-enter {
    0% {
      right: -100%;
    }
    100% {
      right: 0%;
    }
  }
</style>