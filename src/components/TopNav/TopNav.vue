<template>
    <div class="theTopNavWrapper">
        <div class="theLogoWrapper">
            <img class="logo" :src="logo" alt="">
            <img class="trademark" :src="trademark" alt="">
        </div>

        <div class="theNavOptions">
            <div v-for="option in navOptions" :key="option">
                <span class="navOption">{{option}}</span>
            </div>
        </div>
        
        <div class="theNavButtons">
            <Button class="navButton other" simple>CONTACT US</Button>
            <Button class="navButton" >JOIN HYDRA</Button>
        </div>
    </div>
</template>
<script>
import Button from '../shared/button.vue'
import logo from '../../assets/logo.svg'
import trademark from '../../assets/trademark.svg'
export default {
    components:{
        Button
    },
    setup(){
        const navOptions = ['ABOUT','SERVICES','TECHNOLOGIES','HOW TO']
        return{
            logo,
            trademark,
            navOptions,
        }
    }
}
</script>

<style scoped>
    .theTopNavWrapper{
        padding: 50px 84px;
        display: flex;
        justify-content: space-between;
        align-items: center;
        background: rgba(0, 0, 0, 0.8);
        min-width: 1144px;
    }
    .theLogoWrapper{
        display: flex;
        align-items: center;
        opacity: 0.9;
    }
    .theLogoWrapper:hover{
        opacity: 1;
    }
    .theLogoWrapper:active{
        opacity: 0.9;
    }
    .theLogoWrapper .logo{
        margin-right: 15px;
    }
    .theNavOptions{
        width: 27%;
        display: flex;
        justify-content: space-between;
    }
    .navOption{
        font-family: 'Montserrat';
        font-style: normal;
        font-weight: 700;
        font-size: 12px;
        line-height: 15px;
        color: #FFFFFF;
    }
    .navOption:hover{
        border-bottom: 1px solid white;
    }
    .navOption:active{
        border-bottom: none;
    }
    .theNavButtons{
        display: flex;
    }
    .theNavButtons .other{
        margin-left: 0px;
    }
    .navButton{
        width: 155px;
        height: 48px;
        margin-left: 38px;
    }
    @media (max-width: 1275px){
        .theNavOptions{
            width: 310px;
        }
    }
</style>