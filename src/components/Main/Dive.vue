<template>
    <div class="theDiveWrapper">
        <div class="mainWrapper">
            <div class="theTextWrapper">
                <div class="title">
                    <span class="colorful">Dive </span>
                    <span class="whiteSimple">Into the Depths <br> Of </span>
                    <span class="colorful">Virtual Reality</span>
                </div>
                <section class="section">
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore nisl tincidunt eget. Lectus mauris eros in vitae .
                </section>
                <div class="buttons">
                    <Button class="buildButton">BUILD YOUR WORLD</Button>
                    <img class="rightIcon" :src="right">
                </div>
            </div>

            <div class="theImageWrapper">
                <img class="DiveImageOne" :src="DiveImageOne" alt="">
                <img class="Vector1" :src="Vector1" alt="">
                <img class="Vector2" :src="Vector2" alt="">
                <img class="Vector3" :src="Vector3" alt="">
            </div>
        </div>

        <!-- <div class="footerWrapper">
            <div class="partWrapper">
                <img :src="location" alt="">
                <div class="textWrapper">
                    <span class="title">Pay Us a Visit</span>
                    <span class="words">Union St, Seattle, WA 98101, United States</span>
                </div>
            </div>
            <div class="line"></div>
            <div class="partWrapper">
                <img :src="phone" alt="">
                <div class="textWrapper">
                    <span class="title">Give Us a Call</span>
                    <span class="words">(110) 1111-1010</span>
                </div>
            </div>
            <div class="line"></div>
            <div class="partWrapper">
                <img :src="email" alt="">
                <div class="textWrapper">
                    <span class="title">Send Us a Message</span>
                    <span class="words">Contact@HydraVTech.com</span>
                </div>
            </div>
        </div> -->

    </div>
</template>

<script>
import Button from '../shared/button.vue'
import right from '../../assets/right.svg'
import location from '../../assets/location.svg'
import phone from '../../assets/phone.svg'
import email from '../../assets/email.svg'
import DiveImageOne from '../../assets/DiveImageOne.svg'
import Vector1 from '../../assets/Vector1.svg'
import Vector2 from '../../assets/Vector2.svg'
import Vector3 from '../../assets/Vector3.svg'
export default {
    components:{
        Button
    },
    setup(){
        return{
            right,
            location,
            phone,
            email,
            DiveImageOne,
            Vector1,
            Vector2,
            Vector3
        }
    }
}
</script>

<style scoped>
    .theDiveWrapper{
        padding: 0px 84px;
        padding-top: 30.63vh;
        width: 100%;
        height: 100vh;
    }
    .DiveImageOne{
        width: 490px;
        height: 426px;
        border-radius: 100px 100px 100px 240px;
    }
    .theTextWrapper{
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        height: 33.94vh;
    }
    .theTextWrapper .title{
        font-family: 'Montserrat';
        font-style: normal;
        font-weight: 700;
        font-size: 46px;
        line-height: 56px;
        width: 486px;
        height: 116px;
    }
    .theTextWrapper .title .colorful{
        background: linear-gradient(91.57deg, #C0B7E8 -1.02%, #8176AF 36.25%);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
        background-clip: text;
        text-fill-color: transparent;
    }
    .theTextWrapper .section{
        font-family: 'Montserrat';
        font-style: normal;
        font-weight: 400;
        font-size: 16px;
        line-height: 20px;
        color: #FFFFFF;
        width: 450px;
        height: 72px;
    }
    .buttons{
        display: flex;
    }
    .buttons .buildButton{
        width: 214px;
        height: 48px;
        margin-right: 40px;
    }
</style>