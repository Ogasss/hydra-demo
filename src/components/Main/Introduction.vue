<template>
    <div class="theIntroductionWrapper">
        <header class="headerWrapper">
            <div class="leftPart">
                <div class="introductionTitle">INTRODUCTION</div>
                <div class="to">
                    <span class="introductionLittleTittle">TO HYDRA VR</span>
                    <img class="leftLine" :src="leftLine" alt="">
                </div>
            </div>
            <div class="sectionWrapper">
                <div class="introductionSection">
                    Vitae sapien pellentesque habitant morbi tristique senectus et netus et. Feugiatnibh sed pulvinar proin gravida hendrerit lectus. Mi sit amet mauris commodo quis imperdiet massa tincidunt nunc. Viverra aliquet eget sit amet tellus. Ornare lectus sit amet est placerat in. Lectus magna fringilla urna porttitor rhoncus vitae.
                </div>
            </div>
        </header>

        <main class="mainWrapper">
            <img class="IntroductionImageOne" :src="IntroductionImageOne" alt="">
            <div class="textWrappers">
                <div class="introductionTitle">ABOUT</div>
                <div class="introductionLittleTittle">HYDRA VR</div>
                <div class="introductionSection">
                    <div>
                        Eget mi proin sed libero enim sed faucibus turpis. Nisl rhoncus mattis rhoncus urna neque viverra justo. Vivamus at augue eget arcu dictum. Ultrices gravida dictum fusce ut placerat orci. Aenean et tortor at risus viverra adipiscing at in. Mattis aliquam faucibus purus in massa. Est placerat in egestas erat imperdiet sed. Consequat semper viverra nam libero justo laoreet sit amet. Aliquam etiam erat velit scelerisque in dictum non consectetur a. Laoreet sit amet cursus sit amet. Vel eros donec ac odio tempor orci dapibus. Sem nulla pharetra diam sit amet nisl suscipit adipiscing bibendum. Leo a diam sollicitudin tempor.
                    </div>
                </div>
                <Button class="touch">LET'S GET IN TOUCH</Button>
            </div>
        </main>
        
    </div>
</template>

<script>
import leftLine from '../../assets/leftLine.svg'
import IntroductionImageOne from '../../assets/IntroductionImageOne.svg'
import Button from '../shared/button.vue'
export default {
    components:{
        Button
    },
    setup(){
        return{
            leftLine,
            IntroductionImageOne
        }
    }
}
</script>

<style scoped>
    .introductionTitle{
        font-family: 'Montserrat';
        font-style: normal;
        font-weight: 700;
        font-size: 36px;
        line-height: 44px;
        color: #FFFFFF;
    }
    .IntroductionImageOne{
        box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
        border-radius: 100px 240px;
    }
    .introductionLittleTittle{
        font-family: 'Montserrat';
        font-style: normal;
        font-weight: 300;
        font-size: 36px;
        line-height: 44px;
        color: #FFFFFF;
    }
    .introductionSection{
        font-family: 'Montserrat';
        font-style: normal;
        font-weight: 400;
        font-size: 16px;
        line-height: 20px;
        color: #FFFFFF;
        opacity: 0.7;
    }
    .theIntroductionWrapper{
        padding-top: 90px;
    }
    .theIntroductionWrapper .headerWrapper{
        display: flex;
        justify-content: space-between;
    }
    .headerWrapper .sectionWrapper{
        display: flex;
        width: 652px;
        height: 98px;
    }
    .sectionWrapper .introductionSection{
        margin: auto;
    }
    .leftPart .to{
        margin-top: 10px;
    }
    .leftPart .to .leftLine{
        margin-top: -50%;
        position: relative;
        top: 35px;
    }
    .to .introductionLittleTittle{
        margin-right: 30px;
    }



    .theIntroductionWrapper .mainWrapper{
        margin-top: 100px;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
    .mainWrapper .touch{
        width: 214px;
        height: 48px;
    }
    .mainWrapper .introductionSection{
        margin-bottom: 28px;
        width: 630px;
        height: 228px;
        display: flex;
        justify-content: center;
        align-items: center;
    }
    .mainWrapper .introductionTitle{
        margin-bottom: 5px;
    }
</style>