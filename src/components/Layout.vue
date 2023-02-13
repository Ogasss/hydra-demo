<template>
<div class="theLayoutWrapper">
    <div class="theTopNav">
        <TopNav/>
    </div>
    <div class="theMain">
        <Dive/>
        <Introduction/>
        <Why/>
    </div>
</div>
</template>

<script>
import TopNav from './TopNav/TopNav.vue'
import Dive from './Main/Dive.vue'
import Introduction from './Main/Introduction.vue'
import Why from './Main/Why.vue'
import { onMounted } from 'vue'
export default {
    components:{
        TopNav,
        Dive,
        Introduction,
        Why
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
    height: 5597px;
    margin-left: 50%;
    transform: translateX(-50%);
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