<template>
    <div class="theJoinWrapper">
        <div class="theFormWrapper">
            <div class="title">JOIN HYDRA</div>
            <div class="line"></div>
            <div class="littleTitle">Let’s Build YourVR Experience</div>
            <div>
                <input class="input" type="text" placeholder="First Name">
                <input class="input" type="text" placeholder="Last Name">
            </div>
            <div>
                <input class="input" type="text" placeholder="Email">
                <input class="input" type="text" placeholder="Phone Number">
            </div>
            <input class="input long" type="text" placeholder="Subject">
            <textarea cols="30" rows="10" placeholder="Tell Us Something..."></textarea>
        </div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style scoped>
    .theJoinWrapper{
        display: flex;
        justify-content: center;
        align-items: center;
    }
    .theFormWrapper{
        padding: 84px 107px;
        width: 1440px;
        height: 1008px;
        border-radius: 100px;
        background: radial-gradient(50% 50% at 50% 50%, #403A5F 0%, #211E2E 100%);
        display: flex;
        flex-direction: column;
        align-items: center;
    }
    .theFormWrapper .input{
        padding: 27px 42px;
        width: 524px;
        height: 72px;
        border: 2px solid #FFF;
        font-family: 'Montserrat';
        font-style: normal;
        font-weight: 400;
        font-size: 14px;
        line-height: 17px;
        color: #FFFFFF;
        border-radius: 40px;
        margin-right: 10px;
        margin-bottom: 40px;
    }
    .theFormWrapper .long{
        width: 1058px;
    }
    .theFormWrapper .title{
        margin-top: 6px;
        font-family: 'Montserrat';
        font-style: normal;
        font-weight: 700;
        font-size: 36px;
        line-height: 44px;
        color: #FFFFFF;
        margin-bottom: 30px;
    }
    .theFormWrapper .line{
        height: 1px;
        width: 414px;
        background: linear-gradient(270deg, #343045 0%, #C0B7E8 34.9%, #8176AF 68.75%, #343045 100%);
    }
    .theFormWrapper .littleTitle{
        margin-top: 21px;
        font-family: 'Montserrat';
        font-style: normal;
        font-weight: 300;
        font-size: 36px;
        line-height: 44px;
        color: #FFFFFF;
        margin-bottom: 65px;
    }
    .theFormWrapper textarea{
        padding: 27px 42px;
        border: 2px solid #FFF;
        border-radius: 40px;
        background: none;
        font-family: 'Montserrat';
        font-style: normal;
        font-weight: 400;
        font-size: 14px;
        line-height: 17px;
        color: #FFFFFF;
        width: 1058px;
        height: 210px;
        resize: none;
    }
    .theFormWrapper textarea::-webkit-scrollbar{
        display: none;
    }
</style>