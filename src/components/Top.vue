<template>
  <div class="scene">
    <div class="container">
      <div class="your-awesome">
        Your awesome traffic permit consultant.
      </div>

      <a class="btn btn-primary">GET STARTED
        <span style="margin-left: 18px"> 
          <i class="fas fa-long-arrow-alt-right"></i>
        </span>
      </a>

      <div id="car">
        <img src="../assets/mobel.svg">
      </div> 
    </div>        
  </div>
</template>

<script>

export default {
  components: {
    
  }
}
</script>

<style lang="scss">
  .scene {
    position: relative;
    margin-top: -120px;
    margin-bottom: 100px;

    min-height: 1133px;
    background-image: url("../assets/Scene.svg");
    background-repeat: no-repeat;
    background-position: center;
    background-size: cover;

    .container {
      
    }
  }  

  .your-awesome {    
    font-size: 100px;
    line-height: 100px;
    font-weight: 400;
    color: white;
    
    width: 70%;
    padding-top: 160px;
    padding-bottom: 80px;
  }

  #car {
    position: absolute;
    left: 0;
    bottom: -50px;
    opacity: 0;

    &.animate {
      opacity: 1;
      animation-name: car-enter;
      animation-duration: 1.5s; 
    }    
  }

  @keyframes car-enter {
	0% {
		left: -100%;
	}
	100% {
		left: 0%;
	}
}
</style>