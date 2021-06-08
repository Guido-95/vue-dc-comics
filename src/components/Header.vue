<template>
    <div class="wrapper">
        <div class="logo">
           <a href=""> <img src="../assets/img/dc-logo.png" alt="logo DC"> </a> 
        </div>
        <div class="link-header">
            <ul>
                <li v-for="link,contatore in links" :key="contatore" :class=" link.linkCorrente ? 'attivo' : '' ">
                   <a :href="link.indirizzo" :class=" link.linkCorrente ? 'linkAttivo' : '' "> {{link.testo}} </a>
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
                    linkCorrente:true
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
    @import "./style/variabili.scss";

    .wrapper {
        display: flex;
        align-items: center;
        height: 140px; 
    }

    .logo {
        width: 40%;

        img{
            
            width: 18%;
        }
    }

    .link-header {
       height: 100%;
        width: 60%;
        
    }

    ul {
        height: 100%;
        display: flex;

        li {
            display: flex;
            align-items: center;
            height: 100%;
            margin: 0px 12px 12px 12px;

           a {
               font-size: 13px;
               font-weight: 700;
               text-transform: uppercase;
               color: #464646;
           }
        }     
        
        li:hover {
            transition: 0.3s;
            box-shadow: inset 0 -5px 0 0 $colore-principale;  
        }
         li a:hover {
            color: $colore-principale;
            
        }

        
    }

    .attivo {
            
            box-shadow: inset 0 -5px 0 0 $colore-principale; 
        }
        .linkAttivo {
            color: $colore-principale;
        }

</style>