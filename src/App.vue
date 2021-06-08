<template>
  <div id="app">
    
    <header>
       <Header/>
       <Jumbotron/>
    </header>
   
    <main>

      <section class="contenuto-principale wrapper">
        <Prodotto 
        v-for="(prodotto,contatore) in prodotti" :key=" contatore "
        :prodotto="prodotto" />
        
        <button> Load more </button>
        
      </section>

      <section class="contenuto-secondario">
        <SezioneSecondaria/>
      </section>

    </main>
    
    <footer>
      <div class="footer-top">
        <FooterAlto/>
      </div>

      <div class="footer-bottom">
        <FooterBasso/>
      </div>
    </footer>
   
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Jumbotron from './components/Jumbotron.vue'
import Prodotto from './components/Prodotto.vue'
import SezioneSecondaria from './components/SezioneSecondaria.vue'
import FooterAlto from './components/FooterAlto.vue'
import FooterBasso from './components/FooterBasso.vue'


export default {
  name: 'App',
  components: {
    Header : Header,
    Jumbotron : Jumbotron,
    Prodotto : Prodotto,
    SezioneSecondaria: SezioneSecondaria,
    FooterAlto : FooterAlto,
    FooterBasso:FooterBasso
  },
  data () {
    return {
      prodotti : 
      [
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
          "price": "$19.99",
          "series": "Action Comics",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
          "price": "$3.99",
          "series": "American Vampire 1976",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
          "price": "$16.99",
          "series": "Aquaman",
          "type": "graphic novel"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
          "price": "$2.99",
          "series": "Batgirl",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          "price": "$3.99",
          "series": "Batman",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          "price": "$2.99",
          "series": "Batman Beyond",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
          "price": "$3.99",
          "series": "Batman/Superman",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
          "price": "$4.99",
          "series": "Batman/Superman Annual",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
          "price": "$5.99",
          "series": "Batman: The Joker War Zone",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
          "price": "$6.99",
          "series": "Batman: Three Jokers",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
          "price": "$4.99",
          "series": "Batman: White Knight Presents: Harley Quinn",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
          "price": "$16.99",
          "series": "Catwoman",
          "type": "graphic novel"
        }
      ]

    }
  }
}
</script>

<style lang="scss">
   @import "./style/variabili.scss";
  

  * {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
  }

  body {
    font-family: $font-principale;
  }

  
  main {
    background-color: #1c1c1c;

    .contenuto-principale {
      display: flex;
      flex-wrap: wrap;
      padding: 50px 50px 25px 50px;

      button {
        text-transform: uppercase;
        padding: 10px 50px;
        border: none;
        font-weight: 700;
        margin: 25px auto 0px auto;
        background-color: $colore-principale;
        color: white;
      }
    }

    .contenuto-secondario {
      position: relative;
      z-index:3;
      background-color: $colore-principale;
    }
  }
  
  .footer-top {
    height: 380px;
    z-index: 1;
    background-repeat: no-repeat;
    background-size: cover;
    background: url("./assets/img/footer-bg.jpg");
  }

  .footer-bottom {
    position: relative;
    z-index:3;
    background-color: #303030;
  }
  

  .wrapper {
    max-width: 1400px;
    margin: auto;
  }

  ul {
    list-style: none;
  }

  a {
    text-decoration: none;
  }

</style>
