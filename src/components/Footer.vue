<template>

  <div id="footer">

    <div id="truck">
      <img src="@/assets/Group 35.svg" alt=" nu se afiseaza">
    </div>
    <div id="footer-bg">
      <img src="@/assets/BG.svg" alt="bg nu ruleaza">
    </div>
    <div id="vector-bg">
      <img src="@/assets/Vector 13.svg" alt="bg nu ruleaza">
    </div>
    <div class="container">
      <div>
        <div id="text-footer">
          <p>We provide traffic management consultants so you get started quickly, contact us for a quote today!</p>
        </div>
      </div>
      <div>
        <div id="formular">
          <div class="form-input">
            <label>Name</label>
            <input type="text" placeholder="Your name">
          </div>

          <div class="form-input">
            <label>Email</label>
            <input type="text" placeholder="Your email adress">
          </div>
          <div>
            <a class="btn btn-primary">GET STARTED
              <span style="margin-left: 18px"> 
                <i class="fas fa-long-arrow-alt-right"></i>
              </span>
            </a>
          </div>

        </div>
      </div>
    </div>

    <div id="navigation" class="container">
      <div class="logo">
        <img src="../assets/logo.svg" alt="nu se afiseaza logo">
      </div>
      <div class="actions-wraper">
        <div class="actions">
          <a href="#about" class="btn">ABOUT</a>
          <a href="#how-to-apply" class="btn">HOW TO</a>
          <a class="btn">FAQS</a>
        </div>
      </div>
    </div>
    
    <div id="social">
      <div class="container">
        <div id="copyright">Copyright @ 2019 </div>
        <div class="actions">
          <a class="btn btn-icon">
            <i class="fab fa-facebook"></i> 
          </a>
          <a class="btn btn-icon">
            <i class="fab fa-twitter"></i> 
          </a>
          <a class="btn btn-icon">
            <i class="fab fa-instagram"></i>
          </a>
        </div>
      </div>
      
    </div>

  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
  #footer {
    padding-top: 212px;
    position: relative;
    .container {
      padding: 20px 0px;
      display: flex;
      flex-wrap: nowrap;
      align-items: center;
      &>div {
        flex-basis: 50%;
      }
    }
  }

  #text-footer {
    width: 350px;
    border-left: #EE4D47 solid 10px;
    padding: 5px 40px;

    p {
      color: white;
      font-weight: normal;
      font-size: 20px;
      line-height: 30px;
    }

  }
  #formular {
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    width: 550px;
    height: 440px;
    padding: 52px 75px;

    background: #FFFFFF;
    box-shadow: 0px 20px 40px rgba(238, 77, 71, 0.1);
    border-radius: 10px;

    .form-input {
      display: flex;
      flex-direction: column;
      
      input { 
        padding: 11px 20px 11px 40px;
        font-size: 18px;
        height: 60px;
        border: 2px solid #EE4D47;
        box-sizing: border-box;
        border-radius: 5px;
        &:focus {
          box-shadow: 0px 20px 40px rgba(238, 77, 71, 0.2);
        }

      }
       label {
          padding: 10px 0px;
          color: #402B2B;
          font-style: normal;
          font-weight: 300;
          font-size: 16px;
          line-height: 40px;
        }
    }
  } 

  #truck {
    position: absolute;
    top: 115px;
    opacity: 0;

      &.animate {
        opacity: 1;
        animation-name: truck-enter;
        animation-duration: 1.5s; 
      }          
  }

  #navigation {
    padding: 150px 0px !important;
    &.container {
      display: flex;
      justify-content: space-between;
      align-items: center;
      .actions-wraper {
        display: flex;
        justify-content: center;

      }
      .actions {
        display: flex;
        justify-content: space-around;
        width: 368px;
      }
      
    }
  }
  #footer-bg {
    position: absolute;
    z-index: -3;
    top: 300px;
    
    img {
      position: absolute;
      height: 982px;
      transform: translateX(-320px);
    }
    

  }
  #vector-bg {
    z-index: -2;
    position: absolute;
    top: 300px;

    img {
      height: 730px;
      background-size: cover;
    }
  }

  #social {
    background-color: #FEF8F5;
    height: 141px;

    .container {
      display: flex;
      align-items: center;
      height: 100%;
    }

    .actions {
      display: flex;
      justify-content: flex-end;
      gap: 30px;
    }
  }

  @keyframes truck-enter {
    0% {
      left: -100%;
    }
    100% {
      left: 0%;
    }
  }
</style>