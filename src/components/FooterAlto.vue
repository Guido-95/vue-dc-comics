<template>
   <div class="wrapper">
       
       <div class="lista">
            <h2>dc comics</h2>
            <ul>
                <li><a href="">Characters</a></li>
                <li><a href="">Comics</a></li>
                <li><a href="">Movies</a></li>
                <li><a href="">Tv</a></li>
                <li><a href="">Games</a></li>
                <li><a href="">Videos</a></li>
                <li><a href="">News</a></li>
            </ul>
        <h2>Shop</h2>
        <ul>
           <li><a href="">Shop DC</a></li>
           <li><a href="">Shop DC Collectibles</a></li>
        </ul>
        </div>
        <div class="lista">
            <h2>Dc</h2>
            <ul>
              <li><a href="">Terms Of Use</a></li>
              <li><a href="">Privacy policy (New)</a></li>
              <li><a href="">Ad Choices</a></li>
              <li><a href="">Advertising</a></li>
              <li><a href="">Jobs</a></li>
              <li><a href="">Subscriptions</a></li>
              <li><a href="">Talent Workshops</a></li>
              <li><a href="">CPSC Certificates</a></li>
              <li><a href="">Rating</a></li>
              <li><a href="">Shops Helps</a></li>
              <li><a href="">Contact Us</a></li>
            </ul>
        </div>

        <div class="lista">
            <h2>sites</h2>
            <ul>
                
                <li><a href="">DC</a></li>
                <li><a href="">MAD Magazine</a></li>
                <li><a href="">Dc Kids</a></li>
                <li><a href="">DC Universe</a></li>
                <li><a href="">DC Power</a></li>

            </ul>
        </div>
        <div class="logo-dc-footer">
            <img src="../assets/img/dc-logo-bg.png" alt="logo dc footer">
        </div>
       
   </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
    @import "./style/css.scss";

    .wrapper{
        display: flex;
        position: relative;
        
    }
    .lista{
       margin: 20px 30px 0px 0px;
    }
    
  
    ul {
        li {
            a {  
                font-size: 13px;
                color: #959595;

                &:hover {
                    color: $colore-principale;
                }
            } 
        }
    }

    h2 {
        text-transform: uppercase;
        font-size: 20px;
        margin: 10px 10px 10px 0px;
        color: white;
    }

    .logo-dc-footer {
        position: absolute;
        top: -90px;
        right: 0px;
        z-index:2;
    }

   

</style>