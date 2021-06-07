<template>
    <div class="wrapper">
        <div class="logo">
            <img src="../assets/img/dc-logo.png" alt="logo DC">
        </div>
        <div class="link-header">
            <ul>
                <li v-for="link,contatore in links" :key="contatore">
                   <a href=""> {{link.testo}} </a>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    data :function() {
        return {
            links: [
                {
                    testo:"Characters",
                    indirizzo: "#",
                    linkCorrente:false
                },
                {
                    testo:"Comics",
                    indirizzo: "#",
                    linkCorrente:false
                },
                {
                    testo:"Movies",
                    indirizzo: "#",
                    linkCorrente:false
                },
                {
                    testo:"TV",
                    indirizzo: "#",
                    linkCorrente:false
                },
                {
                    testo:"Games",
                    indirizzo: "#",
                    linkCorrente:false
                },
                {
                    testo:"Collectibles",
                    indirizzo: "#",
                    linkCorrente:false
                },
                {
                    testo:"Videos",
                    indirizzo: "#",
                    linkCorrente:false
                },
                {
                    testo:"Fans",
                    indirizzo: "#",
                    linkCorrente:false
                },
                {
                    testo:"News",
                    indirizzo: "#",
                    linkCorrente:false
                },
                {
                    testo:"Shop",
                    indirizzo: "#",
                    linkCorrente:false
                },
                

            ] 
        }
    },
}
</script>

<style lang="scss" scoped>

    .wrapper{
        display: flex;
        align-items: center;
        height: 140px; 
    }

    .logo{
        width: 40%;
       
    }

    .link-header{
        width: 60%;
        
    }

    ul{
        display: flex;
        li {

           a {
               padding: 15px;
           }
        }
    }

</style>