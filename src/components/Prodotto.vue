<template>
    
    <div class="articolo">
        <div class="img">
             <img :src="prodotto.thumb" :alt="prodotto.series">
        </div>
        <span class="nome-prodotto"> {{ prodotto.series }} </span>
       
    </div>
 
    
</template>

<script>
export default {
    name:"prodotto",
    props: {
        prodotto:Object,
    }
}
</script>

<style lang="scss" scoped>
    .articolo {
        flex-direction: column;
        color: white;
        margin: 15px;
        width: calc(100% / 6 - 30px);

        .img {
            height: 185px;
            overflow:hidden;
        }

        .nome-prodotto{
            font-size: 14px;
            text-transform: uppercase;
            display: block;
            margin: 20px 0px 15px 0px;
        }

        &  img {
        display: block;
        cursor: pointer;
        width: 100%; 
         
        &:hover{
            width: 180px;
            margin: auto;
            transition: 0.2s;
        }
        
        }
    }

   

   

</style>