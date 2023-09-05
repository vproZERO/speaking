<template>
    <div class="header__box relative mx-auto bg-blue-500">
        <div class="header__box__content">
            
            
            <div class="header__yellow_img absolute bottom-0 right-0 sm:bottom-0">
                <img src="../../imgs/yellow.svg" alt="yellow">
            </div>
            <div class="header__yellow_img img2 absolute bottom-0 right-0 sm:bottom-0">
                <img src="../../imgs/yellow.svg" alt="yellow">
            </div>
            <div class="header__flag_img absolute left-0 top-0 sm:bottom-0">
                <img src="../../imgs/flag.svg" alt="img">
            </div>
            <div class="header__redphone_img absolute right-20 bottom-0">
                <img src="../../imgs/redphone.svg" alt="img">
            </div>
            <div class="header__tutor absolute bottom-0 right-80 ">
                <img src="../../imgs/tutor.svg" alt="tutor">
            </div>
            <div class="header__asset_img absolute bottom-0 left-0">
                <img src="../../imgs/asset.svg" alt="asset">
            </div>
            <div class="header__tree2_img absolute bottom-0 left-0">
                <img src="../../imgs/tree2.svg" alt="img">
            </div>
            <div class="header__tree_img absolute right-0 bottom-0">
                <img src="../../imgs/tree.svg" alt="tree">
            </div>
    
    
            <div class="header__headline absolute left-56 ">
                <h2 class="res__title uppercase text-white font-extrabold text-9xl">speaking</h2>
                <div class="flex items-center gap-4">
                    <h2 class="res__title uppercase text-amber-300 font-extrabold text-9xl">kursi</h2>
                    <div>
                        <p class=" headline__caveat caveat2 italic -rotate-12 font-normal text-2xl text-center text-white">Speak with</p>
                        <p class=" headline__caveat caveat italic -rotate-12 font-medium text-3xl text-white">confidence</p>
                    </div>
                </div>
    
                <div class=" res__zoom__box flex items-center mt-4 mb-6">
                    <div class="flex items-center">
                        <div class="res__zoom__img">
                            <img src="../../imgs/zoom.svg" alt="zoom">
                        </div>
                        <h2 class="res_zoom_text font-medium text-lg text-white w-28">darslar <span class="font-bold">zoom platformasida</span> bo`lib o`tadi</h2>
                    </div>
                    <div class="flex items-center">
                        <div class="res__zoom__img">
                            <img src="../../imgs/calendar.svg" alt="zoom">
                        </div>
                        <div>
                            <h2 class="res_zoom_text font-medium text-lg text-white ">Kurs davomiyligi</h2>
                            <p class="res_zoom_text font-bold text-lg text-white " >1.5 oy</p>
                        </div>
                    </div>
                </div>
    
                <div>
                    <div class="res__som__box p-2 bg-blue-400 rounded-lg w-64 mx-auto flex items-center">
                        <h2 class="text-2xl text-blue-300 font-bold line-through decoration-white">249 000</h2>
                        <h2 class="text-3xl text-white font-bold ">149 000</h2>
                        <p class="-rotate-90 text-white">so`m</p>
                    </div>
                    <div  class="headling__btn mx-auto">
                        <button v-on:click="isOpen = !isOpen" class=" bg-amber-300 py-2 px-6 rounded-lg text-xl font-bold uppercase hover:bg-amber-200 mb-4">chegirmada sotib olish</button>
                        <Modal  :class="isOpen ? 'block' : 'hidden'"   class=" bg-black bg-opacity-25 fixed inset-0 z-50 mx-auto "/>
                    </div>

                    <p class="headline__caveat caveat3 text-md italic text-center text-white"><span class="text-amber-300">Ulgurib qoling,</span> Joylar soni cheklangan!</p>
                </div>
            </div>
    
            <div class="header__email absolute right-1/3 bottom-40">
                <div class="res__email rounded-lg bg-white p-2">
                    <p class="res__volida text-blue-500 text-md text-center font-bold">Volida Matkarimova</p>
                    <p class="headline__caveat italic text-center">English Teacher</p>
                </div>
                <button class="flex items-center bg-opacity-90 gap-2 bg-gray-500 rounded-lg p-2 w-28 mx-auto">
                    <div class="" >
                        <img src="../../imgs/instagramm.svg" alt="instagramm">
                    </div>
                    <a class="underline text-white" target="blank" href="https://www.instagram.com/volida_edu/">volida_edu</a>
                </button>
            </div>

        </div>
    </div>
</template>
<script>
import Modal from '../modal/modal.vue'
export default {
    components: {
        Modal
    },
    data : () => {
        return {
            isOpen : false,
            onOpen : false,
        }
    }
}
</script>
<style scoped>
    .header__box{
        width: 1470px;
        height: 700px;
        margin: 0 auto;
    }
    .header__box__content{
        width: 1471px;
    }
    .header__flag_img{
        width: 311px;
        height: 357px;
    }
    .header__yellow_img{
        width: 660px;
        height: 720px;
    }
    .header__redphone_img{
        height: 591px;
        width: 466px;
    }
    .header__tutor{
        width: 492px;
        height: 591px;
    }
    .headling__btn{
        max-width: 340px;
    }
    .header__tree2_img{
        width: 350px;
        height: 341px;
    }
    .header__tree_img{
        width: 350px;
        height: 341px;
    }
    .headline__caveat{
        font-family: 'Caveat', cursive;
    }
    @media screen and (max-width: 390px){
        .modal__box{
            width: 350px;
            height: 300px;
            margin: 0 auto;
            padding: 10px;
            margin-bottom: 40px;
        }
        .modal__input{
            width: 310px;
            height: 30px;
            padding: 5px ;
            margin-bottom: 5px;
        }
        .modal__btn{
            width: 310px;
            height: 44px;
            padding: 12px 114px;
        }
        .modal__btn2{
            width: 310px;
            height: 30px;
            padding: 0 ;
            font-size: 16px;
            line-height: 18px;
        }
        .res__modal__title{
            width: 233px;
            font-size: 16px;
            line-height: 16px;
            margin: 0 auto;
            padding-top: 15px;
            margin-bottom: 5px;
        }
        .res__modal_subtitle{
            width: 64px;
            margin: 0 auto;
            margin-bottom: 5px;
        }
        .res__modal__num{
            width: 145px;
            font-size: 16px;
            line-height: 20px;
            
        }
        .res__modal_subsom{
            width: 106px;
            margin: 0 auto;
            font-size: 16px;
            line-height: 16px;
            margin-bottom: 5px;
        }
        .header__box__content{
            background-color: #3b82f6;
            position: relative;
            width: 390px;
            height: 700px;
            overflow: hidden;
            margin: 0 auto;
        }
        .header__box{
            background-color: white;
        }
        .res__title{
            width: 359px;
            font-size: 66px;
            line-height: 1;
            margin: 0 auto;
            margin-left: -200px;
        }
        .header__yellow_img{
            position: absolute;
            bottom: -200px;
            left: -59px;
            width: 400px;
            height: 400px;
        }
        .header__tree2_img{
            width: 109px;
            height: 108px;
        }
        .header__tree_img{
            width: 109px;
            height: 108px;
        }
        .header__redphone_img{
            width: 177px;
            height: 315px;
            top: 365px;
            right: -40px;
        }
        .header__flag_img{
            position: absolute;
            width: 344px;
            height: 199px;
            top: 430px;
            left: -70px;
        }
        .header__tutor{
            position: absolute;
            width: 349px;
            height: 447px;
            margin-right: -300px;
            margin-bottom: -130px;
            
        }
        .header__email{
            width: 203px;
            height: 46px;
            top: 580px;
            left: 90px;
        }
        .res__volida{
            width: 151px;
            margin: 0 auto;
            margin-bottom: 0;
        }
        .res__email{
            width: 203px;
        }
        .caveat2{
            width: 74px;
            font-size: 20px;
            margin-left: -160px;
        }
        .caveat{
            width: 104px;
            font-size: 30px;
            margin-left: -160px;
        }
        .res__zoom__box{
            margin-left: -200px;
        }
        .res__zoom__img{
            width: 56px;
            height: 56px;
        }
        .res_zoom_text{
            width: 96px;
            font-size: 12px;
            line-height: 16px;
        }
        .res__som__box{
            width: 227px;
            height: 55px;
            margin-left: -150px;
        }
        .headling__btn{
            width: 350px;
            font-size: 16px;
            line-height: 24px;
            margin-left: -180px;
            margin-block: 0;
        }
        .caveat3{
            width: 305px;
            font-size: 24px;
            line-height: 32px;
            margin-left: -180px;
        }
    }
    
</style>