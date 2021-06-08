<template>
   
    
    <div class="jumbotron">
        <img src="../assets/img/jumbotron.jpg" alt="jumbotron">
        <span>Current series</span>
    </div>
        
 
   
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
    @import "./style/css.scss";
    .wrapper {
        height: 160px;
        display: flex;
        align-items: center;
        font-size: 30px;
        color: white;  
    }

    .jumbotron {
        position: relative;
        height: 400px;
        width: 100%;

        img {
            height: 100%;
            width: 100%;
            object-fit: cover;
            object-position: 0px 0px;
        }

        span {
            position: absolute;
            bottom: -30px;
            left: 305px;
            font-size: 25px;
            background-color: $colore-principale;
            padding: 15px 30px;
            font-weight: 700;
            text-transform: uppercase;
            color: white;
        }


    }

   
</style>