<template>
  <div id="how-to-apply">
    <div class="container">

      <div id="lady">
        <img src="@/assets/illustrations.svg"/>
      </div>

      <div></div>

      <div class="how-to-apply-text">
        <div class="title">How to apply</div>

        <p>
          When applying for a traffic permit, there are certain requirements that you must meet that are included in the examination: requirements for professional knowledge, solid establishment, good reputation and financial resources. Important to remember is to confirm your application for a traffic permit by the company's company signer or CEO.
        </p>
      </div>      
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
  #how-to-apply {
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

      .how-to-apply-text {
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
      }

      #lady {
        position: absolute;
        left: 0;
        opacity: 0;

        &.animate {
          opacity: 1;
          animation-name: lady-enter;
          animation-duration: 2s; 
        }        

        img {
          height: 550px;
        }
      }
  }

  @keyframes lady-enter {
    0% {
      left: -100%;
    }
    100% {
      left: 0%;
    }
  }
</style>