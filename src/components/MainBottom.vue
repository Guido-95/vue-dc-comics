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
        justify-content: center;
      
    }

    img{
        margin-right: 10px;
        height: 45px;
    }

    .img{
        margin-left: 25px;
        display: flex;
        align-items: center;
        width: calc(88% / 5);
        text-transform: uppercase;
        color: white;
        font-size: 15px;
        
    }

    
</style>