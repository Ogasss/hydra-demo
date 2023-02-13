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
                <div class="vectorWrapper">
                    <img class="Vector1" :src="Vector1" alt="">
                    <img class="Vector2" :src="Vector2" alt="">
                    <img class="Vector3" :src="Vector3" alt="">
                </div>
            </div>
        </div>

        <div class="footerWrapper">
            <div class="partWrapper">
                <img :src="location" alt="">
                <div class="textWrapper">
                    <div class="title">Pay Us a Visit</div>
                    <div class="words">Union St, Seattle, WA 98101, United States</div>
                </div>
            </div>
            <div class="line"></div>
            <div class="partWrapper">
                <img :src="phone" alt="">
                <div class="textWrapper">
                    <div class="title">Give Us a Call</div>
                    <div class="words">(110) 1111-1010</div>
                </div>
            </div>
            <div class="line"></div>
            <div class="partWrapper">
                <img :src="email" alt="">
                <div class="textWrapper">
                    <div class="title">Send Us a Message</div>
                    <div class="words">Contact@HydraVTech.com</div>
                </div>
            </div>
        </div>
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
        padding-top: 30.63vh;
        width: 100%;
        overflow: auto;
    }
    .theDiveWrapper::-webkit-scrollbar{
        display: none;
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
        z-index: 2;
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
    .mainWrapper{
        display: flex;
        justify-content: space-between;
    }

    .theImageWrapper .DiveImageOne{
        position: relative;
        z-index: 2;
    }
    .Vector1{
        position: absolute;
        top: 180px;
        right: 0px;
        z-index: 1;
    }
    .Vector2{
        position: absolute;
        top: 0px;
        right: 134px;
        z-index: 1;
    }
    .Vector3{
        position: absolute;
        top: 419px;
        right: 0;
        z-index: 1;
    }

    .footerWrapper{
        padding: 54px;
        margin-top: 103px;
        height: 164px;
        display: flex;
        justify-content: space-between;
        align-items: center;
        background: radial-gradient(50% 2900.76% at 50% 53.89%, rgba(58, 52, 86, 0.95) 0%, #211E2E 100%);
        border-radius: 90px;
        position: relative;
        z-index: 2;
    }
    .footerWrapper .partWrapper{
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
    .footerWrapper .line{
        border: 1px solid #C0B7E854;
        height: 116.5px;
    }
    .partWrapper .textWrapper{
        margin-left: 25px;
    }
    .partWrapper .textWrapper .title{
        font-family: 'Montserrat';
        font-style: normal;
        font-weight: 700;
        font-size: 24px;
        line-height: 29px;
        color: #FFFFFF;
    }
    .partWrapper .textWrapper .words{
        font-family: 'Montserrat';
        font-style: normal;
        font-weight: 400;
        font-size: 14px;
        line-height: 17px;
        color: #FFFFFF;
    }
</style>