<template>
    <div class="p-10 bigbox">
        <h2 class="kimlar__title uppercase text-4xl font-bold mb-5 text-center mt-10">kurs <span class="text-blue-600">kimlar uchun?</span></h2>
        <div class="kimlar__box mx-auto flex items-start gap-5">
            <div class=" mb-5">
                <div class="kimlar__pink_box p-5 rounded-lg bg-pink-200 flex items-center gap-12 mb-5">
                    <h2 class="text-lg font-mixed kimlar__text">Grammatika qoidarini bilasiz, <span class="font-bold">lekin so’zlasha olmaysiz</span></h2>
                    <div class="kimlar__img">
                        <img src="../../imgs/monkey.svg" alt="monkey">
                    </div>
                </div>
                <div class="kimlar__pink_box p-5 rounded-lg bg-blue-200 flex items-center gap-24 mb-5">
                    <h2 class="text-lg font-mixed w-96 kimlar__text"><span class="font-bold">Kichik yoshli farzandlaringizga</span> mustaqil ingliz tilida gapirishni o’rgatmoqchisiz</h2>
                    <div class="kimlar__img">
                        <img src="../../imgs/family.svg" alt="family">
                    </div>
                </div>
                <div class="kimlar__pink_box p-5 rounded-lg bg-pink-200 flex items-center gap-12 mb-5">
                    <h2 class="text-lg font-mixed kimlar__text"><span class="font-bold">Ishlamoqchi bo’lgan ishingizda</span> ingliz tilini talab qilsa</h2>
                    <div class="kimlar__img">
                        <img src="../../imgs/chemodan.svg" alt="chemodan">
                    </div>
                </div>
            </div>
            <div class=" mb-5">
                <div class="kimlar__pink_box p-5 rounded-lg bg-blue-200 flex items-center gap-12 mb-5">
                    <h2 class="text-lg font-mixed kimlar__text"><span class="font-bold">Ingliz tilidagi kino va qo’shiqlarni tushunib</span> ko’rishni va eshitishni xohlaysiz</h2>
                    <div class="kimlar__img">
                        <img src="../../imgs/tv.svg" alt="tv">
                    </div>
                </div>
                <div class="kimlar__pink_box p-5 rounded-lg bg-pink-200 flex items-center gap-12  mb-5  ">
                    <h2 class="kimlar__text text-lg font-mixed">Chet elga ketmoqchisiz, lekin sizga <span class="font-bold">til bilmaslik to’sqinlik qilayapti</span></h2>
                    <div>
                        <img src="../../imgs/airplane.svg" alt="airplane">
                    </div>
                </div>
            </div>
        </div>
        <div class=" items-center gap-5 mb-10">
            <h2 class="respons__subtitle text-center text-2xl font-bold mb-1.5">Sizda ham xuddi shunday holatmi?</h2>
            <p class="headline__caveat italic text-center text-lg text-blue-600 mb-1.5">Unday bo‘lsa, ushbu kurs aynan siz uchun!</p>
            <div class="w-80 mx-auto mb-10">
                <button v-on:click="isOpen = !isOpen"  class="bg-amber-300 rounded-lg py-3 px-12 text-base font-bold uppercase hover:bg-amber-200">chegirmada sotib olish</button>
                <Modal  :class="isOpen ? 'block' : 'hidden'"   class=" bg-black bg-opacity-25 fixed inset-0 z-50 mx-auto "/>
            </div>
        </div>
    </div>
</template>
<script>
import Modal from '../modal/modal.vue'
export default {
    components : {
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
.headline__caveat{
        font-family: 'Caveat', cursive;
    }
.kimlar__box{
    width: 1216px;
}
    .kimlar__pink_box{
        width: 598px;
        height: 112px;
    }
    .kimlar__img{
        width: 72px;
        height: 72px;
    }
    .kimlar__text{
        width: 481px;
    }
    
    .bigbox{
        width: 1470px;
        margin: 0 auto;
    }
    
    @media screen and (max-width: 390px){
        .kimlar__title{
            width: 349px;
            margin: 0 auto;
            font-size: 24px;
            line-height: 32px;
            margin-block: 20px;
        }
        .kimlar__box{
            display: block;
            margin: 0 auto;
            width: 350px;
        }
        .kimlar__pink_box{
            width: 350px;
        }
        .kimlar__text{
            font-size: 16px;
            line-height: 24px;
        }
        .respons__subtitle{
            font-size: 18px;
            line-height: 28px;
            margin-block: 5px;
        }
        .headline__caveat{
            font-size: 20px;
            line-height: 28px;
        }
        
    }
</style>