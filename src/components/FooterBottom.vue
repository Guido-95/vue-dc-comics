<template>
    <div class="wrapper">
        <div class="footer-left">
             <button>sign-up now!</button>    
        </div>

        <div class="footer-right">
            <span> Follow us </span> 
            <img src="../assets/img/footer-facebook.png" alt="facebook">
            <img src="../assets/img/footer-twitter.png" alt="twitter">
            <img src="../assets/img/footer-youtube.png" alt="youtube">
            <img src="../assets/img/footer-pinterest.png" alt="pinterest">
            <img src="../assets/img/footer-periscope.png" alt="periscope">

            
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
        height: 107px;
        display: flex;
        align-items: center;
      
    }

    .footer-left{
        width: 60%;
     
    }

    .footer-right{
        width: 40%;
        display: flex;
        align-items: center;
        justify-content:flex-end;
    }

    .footer-right > span{
        font-size: 20px;
        text-transform: uppercase;
        font-weight: 700;
        margin-right: 15px;
        color: $colore-principale;
    }

    img{
        cursor: pointer;
        margin: 10px;
    }

    img:hover{
        transition: 0.5s;
        opacity: 70%;
    }
    


    button{
        font-weight: 500;
        font-size: 18px;
        text-transform: uppercase;
        padding: 10px 15px;
        background: none;
        cursor: pointer;
        border: 2px solid $colore-principale;
        color: white;
    }

    button:hover{
        background:$colore-principale;
        color: white;
        transition: 0.5s;
        
    
    }
    
</style>