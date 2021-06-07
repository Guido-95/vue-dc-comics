<template>
  <div id="app">
    
    <header>
       <Header/>
    </header>
   
    <main>

      <section class="contenuto-principale">
        <Main/> 
      </section>

      <section class="contenuto-secondario">
        <MainBottom/>
      </section>

    </main>
    
    <footer>
      <div class="footer-top">
        <Footer/>
      </div>

      <div class="footer-bottom">
        <FooterBottom/>
      </div>
    </footer>
   

  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import MainBottom from './components/MainBottom.vue'
import Footer from './components/Footer.vue'
import FooterBottom from './components/FooterBottom.vue'


export default {
  name: 'App',
  components: {
    Header : Header,
    Main : Main,
    MainBottom: MainBottom,
    Footer : Footer,
    FooterBottom:FooterBottom
  }
}
</script>

<style lang="scss">
  *{
    box-sizing: border-box;
    margin: 0;
    padding: 0;
  }

  
  main{
    .contenuto-principale{
    
    background-color: black;
    }
    .contenuto-secondario {
      
      background-color: rgb(128, 217, 247);
    }
   
  }
  
  .footer-top{
    height: 380px;
    
    background: url("./assets/img/footer-bg.jpg");
    
    background-repeat: no-repeat;
    background-size: cover;
  }
  

  .wrapper{
    max-width: 1170px;
    margin: auto;
    border: 1px solid red;
    
  }

  ul{
    list-style: none;
  }

</style>
