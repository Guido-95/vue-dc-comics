<template>
   <div class="wrapper">
       <div class="img">
            <img src="../assets/img/buy-comics-digital-comics.png" alt="">
            digital comics
        </div>
        <div class="img">

            <img src="../assets/img/buy-comics-merchandise.png" alt="">
            dc merchandise
        
        </div>
        <div class="img">
            <img src="../assets/img/buy-comics-subscriptions.png" alt="">
            subscription
        </div>
        <div class="img">
            <img src="../assets/img/buy-comics-shop-locator.png" alt="">
            comic shop locator
        </div>

        <div class="img">
            <img src="../assets/img/buy-dc-power-visa.svg" alt="">
            dc power visa
        </div>


    </div>
</template>

<script>
export default {

}
</script>

<style scoped>
    .wrapper {
        height: 150px;
        display: flex;
        align-items: center;
        justify-content: space-around;
      
    }

    img{
        height: 50px;
    }

    .img{
        display: flex;
        align-items: center;
        width: calc(88% / 5);
        border: 1px solid black;
    }

    
</style>