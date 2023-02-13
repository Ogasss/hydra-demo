<template>
    <div class="theLinksWrapper">
        <img class="logo" :src="logo" alt="">
        <div class="line one"></div>
        <div class="links">
            <div v-for="link in linksList1" :key="link">
                <span class="link">{{link}}</span>
            </div>
        </div>
        <div class="line two"></div>
        <div class="links">
            <div v-for="link in linksList2" :key="link">
                <span class="link">{{link}}</span>
            </div>
        </div>
        <div class="line three"></div>
        <div class="other">
            <div class="title">SOCIALIZE WITH HYDRA</div>
            <div class="icons">
                <div v-for="iconSrc in icons" :key="iconSrc">
                    <img class="icon" :src="iconSrc" alt="">
                </div>
            </div>
            <Button class="button">BUILD YOUR WORLD</Button>
        </div>
        <img class="Vector V18" :src="Vector18" alt="">
        <img class="Vector V19" :src="Vector19" alt="">
    </div>
</template>

<script>
import logo from '../../assets/logo.svg'
import facebook from '../../assets/facebook.svg'
import twitter from '../../assets/twitter.svg'
import linkedin from '../../assets/linkedin.svg'
import youtube from '../../assets/youtube.svg'
import instagram from '../../assets/instagram.svg'
import pinterest from '../../assets/pinterest.svg'
import Vector18 from '../../assets/Vector18.svg'
import Vector19 from '../../assets/Vector19.svg'

import Button from '../shared/button.vue'

export default {
    components:{
        Button
    },
    setup(){
        const linksList1 = [
            'ABOUT',
            'SERVICES',
            'TECHNOLOGIES',
            'HOW TO',
            'JOIN HYDRA'
        ]
        const linksList2 = [
            'F.A.Q',
            'SITEMAP',
            'CONDITIONS',
            'LICENSES',
        ]
        const icons = [
            facebook,
            twitter,
            linkedin,
            youtube,
            instagram,         
            pinterest,
            
        ]
        return{
            logo,
            linksList1,
            linksList2,
            icons,
            Vector18,
            Vector19
        }
    }
}
</script>

<style scoped>
    .theLinksWrapper{
        margin-top: 130px;
        margin-bottom: 80px;
        display: flex;
        justify-content: center;
    }
    .theLinksWrapper .logo{
        width: 185px;
        height: 186px;
        margin-right: 100px;
    }
    .theLinksWrapper .line{
        width: 3px;
        height: 196px;
        background: linear-gradient(179.87deg, #343045 0.47%, #343045 0.47%, #C0B7E8 35.21%, #8176AF 68.91%, #343045 99.5%);
    }
    .theLinksWrapper .one{
        margin-right: 81px;
    }
    .theLinksWrapper .two{
        margin-right: 107px;
    }
    .theLinksWrapper .three{
        margin-right: 71px;
    }
    .theLinksWrapper .links{
        display: flex;
        flex-direction: column;
        margin-right: 104px;
        justify-content: space-between;
    }
    .theLinksWrapper .link{
        font-family: 'Montserrat';
        font-style: normal;
        font-weight: 700;
        font-size: 16px;
        line-height: 20px;
        color: #FFFFFF;
    }
    .theLinksWrapper .link:hover{
        border-bottom: 1px solid rgb(150, 150, 150);
    }
    .theLinksWrapper .link:active{
        border-bottom: none;
    }
    .other{
        display: flex;
        flex-direction: column;
        justify-content: space-between;
    }
    .other .button{
        width: 214px;
        height: 48px;
    }
    .other .title{
        font-family: 'Montserrat';
        font-style: normal;
        font-weight: 700;
        font-size: 16px;
        line-height: 20px;
        color: #FFFFFF;
    }
    .other .icons{
        display: flex;
        justify-content: space-between;
    }
    .other .icons .icon{
        margin-right: 20px;
    }
    .theLinksWrapper .Vector{
        position: absolute;
        z-index: -1;
    }
    .V18{
        margin-top: -43px;
    }
    .V19{
        margin-top: -323px;
    }
</style>