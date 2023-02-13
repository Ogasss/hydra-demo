<template>
<div class="theLayoutWrapper">
    <div class="theTopNav">
        <TopNav/>
    </div>
    <div class="theMain">
        <Dive/>
        <Introduction/>
        <Why/>
        <Technologies/>
        <How/>
        <Join/>
        <Links/>
        <Footer/>
    </div>
</div>
</template>

<script>
import TopNav from './TopNav/TopNav.vue'
import Dive from './Main/Dive.vue'
import Introduction from './Main/Introduction.vue'
import Why from './Main/Why.vue'
import Technologies from './Main/Technologies.vue'
import How from './Main/How.vue'
import Join from './Main/Join.vue'
import Links from './Main/Links.vue'
import Footer from './Main/Footer.vue'

import { onMounted } from 'vue'
export default {
    components:{
        TopNav,
        Dive,
        Introduction,
        Why,
        Technologies,
        How,
        Join,
        Links,
        Footer
    },
    setup(){
        let scrollTop = 0
        // let table = {
        //     Dive: 0,
        //     Introduction: 600,
        //     Why: 1500,
        // }
        const scrollToTop = (scrollTop) => { 
            scrollTop = window.pageYOffset || document.documentElement.scrollTop || document.body.scrollTop;
            console.log(scrollTop)
        }
        onMounted(()=>{
            window.addEventListener('scroll', ()=>{scrollToTop(scrollTop)})
        })
    }
}
</script>

<style scoped>
.theLayoutWrapper{
    width: 100%;
    min-width: 1485px;
    /* height: 5597px; */
}
.theTopNav{
    position: fixed;
    top: 0px;
    width: 100%;
    z-index: 2;
}
.theMain{
    padding: 0px 84px;
    position: relative;
    z-index: 1;
}
</style>