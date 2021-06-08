<template>
   <div class="wrapper">
       <div class="img">
            <a href="#">
               <img src="../assets/img/buy-comics-digital-comics.png">
               
            </a>
            digital comics
        </div>
        <div class="img">
            <a href="">
                <img src="../assets/img/buy-comics-merchandise.png">
            </a>
           
            dc merchandise
        
        </div>
        <div class="img">
            <a href="">
                <img src="../assets/img/buy-comics-subscriptions.png">
            </a>
            
            subscription
        </div>
        <div class="img">
            <a href="">
                 <img src="../assets/img/buy-comics-shop-locator.png">
            </a>
           
            comic shop locator
        </div>

        <div class="img">
            <a href="">
                <img src="../assets/img/buy-dc-power-visa.svg">
            </a>
            
            dc power visa
        </div>


    </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>

    .wrapper {
        height: 150px;
        display: flex;
        align-items: center;
        justify-content: center;
        padding: 10px 100px;
        
        .img {
            margin-left: 25px;
            display: flex;
            align-items: center;
            font-size: 15px;
            width: calc(100% / 5);
            text-transform: uppercase;
            color: white;
           

            img {
                margin-right: 10px;
                height: 45px;
                &:hover{
                    height: 50px;
                    transition: 0.2s;
                }
            }
        }
    }

   
    

    
</style>