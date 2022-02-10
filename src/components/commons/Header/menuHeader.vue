<template>
    <div>
        <ul class="listamenu">
            <li 
            v-for="(elemento, indice) in menuArr" :key="indice" >
                <a 
                @click="currentAct = indice"
                :class="{active : indice == currentAct}"
                href="#">{{elemento.select}}</a>
            </li>
            <!-- <li>
                <a href="">Pages</a>        
            </li>
            <li>
                <a href="">Portfolio</a>
            </li>
            <li>
                <a href="">Blog</a>
            </li>
            <li>     
                <a href="">Shop</a>
            </li>
            <li>     
                <a href="">Elements</a>
            </li> -->
            <li>     
                <a href="">
                    <img src="../../../studio/svg/svg-1.svg" alt="">
                </a>
            </li>
        </ul>
    </div>

</template>

<script>
export default {
    name : "menuHeader",
    data(){
        return {
            currentAct : 0,
            menuArr  : [
                {
                    select : "Home"
                },
                {
                    select : "Pagina"
                },
                {
                    select : "Portfolio"
                },
                {
                    select : "Blog"
                },
                {
                    select : "Shop"
                },
                {
                    select : "Elements"
                }

            ]
        }
    },
    // methods : {
    //     clickActive(actClick){
    //             console.log(actClick)
    //         actClick.target.classList.toggle("active")        },
    // }
}
</script>

<style scoped lang="scss">

@import "../../../assets/style/vars.scss";

.listamenu{
  display: flex;
  justify-content: center;

    li{
        list-style-type: none;
        margin: 10px 20px;
        font-size: 0.8rem;

        a{
        text-decoration: none;
        color: $secondColor;

            img{
                width: 15px;
                height: 15px;
            }
        }
    }
}


</style>