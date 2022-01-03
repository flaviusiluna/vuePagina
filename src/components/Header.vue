<template>
  <div id="header">
    <div class="container">
      <div class="logo">
        <img src="../assets/logo.png" @click="goToTop()">
      </div>

      <div class="navigation">
        <a href="#about" class="btn">ABOUT</a>
        <a href="#how-to-apply" class="btn">HOW TO</a>
        <a class="btn">FAQS</a>
        <a class="btn btn-primary">CONTACT US</a>
      </div>
    </div>
    
  </div>
</template>

<script>
export default {
  methods: {
    goToTop() {
      window.scrollTo(0, 0);
    },
  }
}
</script>

<style lang="scss">
  #header {
    position: sticky;
    z-index: 2147483647;
    width: 100%;    
    padding: 30px 0;

    &.scrolled {
      top: 0px;
      background: #f37e67;
      padding: 10px 0;      
      box-shadow: 0px 0px 28px 6px #f37e67;
    }

    .container {
      display: flex;
      align-items: center;
      justify-content: space-between;
    }
  }

  .logo {
    cursor: pointer;
  }

  .navigation {    
    width: 604px;
    height: 60px;

    display: flex;
    justify-content: space-between;
    align-items: center;   
  }
</style>
