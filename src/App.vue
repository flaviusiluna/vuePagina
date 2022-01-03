<template>
  <div id="app">
    <Header/>
    <Top id="top"/>
    <About id="about"/>
    <HowToApply/>
    <Faq/>
    <Footer/>
  </div>
</template>

<script>
import Top from './components/Top.vue';
import About from './components/About.vue';
import HowToApply from './components/HowToApply.vue';
import Faq from './components/Faq.vue';
import Footer from './components/Footer.vue';
import Header from './components/Header.vue';

export default {
  name: 'App',
  components: {
    Header,
    Top,
    About,
    HowToApply,
    Faq,
    Footer
  },

  created () {
    window.addEventListener('scroll', this.handleScroll);
  },  

  methods: {    
    handleScroll () {
      const header = document.getElementById('header');
      if (window.pageYOffset >= 120) {        
        header.classList.add('scrolled');
      } else if (window.pageYOffset < 50){
        header.classList.remove('scrolled');
      }

      if (window.pageYOffset > 130 && window.pageYOffset < 860) {
        const car = document.getElementById('car');
        car.classList.add('animate');
      }

      if (window.pageYOffset > 860 && window.pageYOffset < 1500) {
        const instructor = document.getElementById('instructor');
        instructor.classList.add('animate');
      }

      if (window.pageYOffset > 860) {
        const lady = document.getElementById('lady');
        lady.classList.add('animate');
      }

      if (window.pageYOffset > 1000) {
        const truck = document.getElementById('truck');
        truck.classList.add('animate');
      }
    }
  },

  destroyed () {
    window.removeEventListener('scroll', this.handleScroll);
  }
}
</script>

<style lang="scss">
  body {
    font-family: sans-serif;
    margin: 0;
    background: #FEF8F5;
  }
</style>
