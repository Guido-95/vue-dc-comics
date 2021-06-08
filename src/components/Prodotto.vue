<template>
    
    <div class="articolo">
        <div class="img">
             <img :src="percorso" :alt="nome">
        </div>
        <span class="nome-prodotto"> {{ nome }} </span>
       
    </div>
 
    
</template>

<script>
export default {
    name:"prodotto",
    props: {
        percorso:String,
        nome:String
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
            height: 180px;
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
        width: 100%;  
        
    }
    }

   

   

</style>