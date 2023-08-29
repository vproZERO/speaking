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
                <div :class="isOpen ? 'block' : 'hidden'"   class=" bg-black bg-opacity-25 fixed inset-0 z-50   mx-auto ">
                    <div class="modal__box flex justify-center items-center mb-2.5 mt-2.5">
                                
                                <div class="modal__box kursga__tolov__btn  mx-auto rounded-lg bg-white p-3">
                                    <button v-on:click="isOpen = !isOpen"  class="absolute" ><span >x</span></button> 
                                <h2 class="res__modal__title text-center font-bold text-lg uppercase mb-5">kursga <span class="text-blue-600">to`lov qilish</span></h2>
                                <div class="modal__input rounded-lg bg-blue-600 bg-opacity-25 py-3 px-5 flex items-center justify-between mb-5">
                                    <h2 class="res__modal__num text-base font-medium text-black">4790 9122 1022 9003</h2>
                                    <div class="w-10 h-3">
                                        <img src="../../imgs/visa.svg" alt="visa">
                                    </div>
                                </div>
                                <div class="modal__input rounded-lg bg-blue-600 bg-opacity-25 py-3 px-5 flex items-center justify-between mb-5">
                                    <h2 class="res__modal__num text-base font-medium text-black">8600 0201 4244 6215</h2>
                                    <div class="w-10 h-3">
                                        <img src="../../imgs/uzcard.svg" alt="visa">
                                    </div>
                                </div>
                                <p class="res__modal_subtitle text-sm text-center font-normal opacity-25">Kurs narxi:</p>
                                <p class="res__modal_subsom font-bold text-base text-center mb-5">149 000 so‘m</p>
                                <button v-on:click="onOpen = !onOpen" class="modal__btn2 bg-amber-300 rounded-lg py-3 px-44">
                                    <p class="uppercase text-center text-base font-bold">skrinshotni yuborish</p>
                                </button>
                                
                                </div>
                    </div>
                </div>
                <div  :class="onOpen ? 'block' : 'hidden'"   class=" bg-black bg-opacity-25 fixed inset-0 z-50 pt-2.5  mx-auto ">
                    <div class="modal__box flex justify-center items-center ">
                        
                        <div class="modal__box mx-auto rounded-lg bg-white p-3">
                                <button v-on:click="onOpen = !onOpen"  class="absolute" ><span >x</span></button>
                                <p class="res__modal__text2 text-center text-xs font-normal mb-1">Menejerdan ma’lumot olish uchun</p>
                                <p class="res__modal__title2 text-blue-600 text-lg font-bold text-center uppercase mb-5">raqamingizni qoldiring</p>
                                <input type="text"  placeholder="Ismingiz" class="py-4 pl-4 modal__input border-2 rounded-xl border-gray-200 block mb-5 " required>
                                <input type="tel" placeholder="Telefon raqamingiz" class="py-4 pl-4 modal__input border-2 rounded-xl border-gray-200 block mb-5" required>
                                <div class="pb-5 modal__input">
                                    <button type="button" class="modal__btn modal__btn2 bg-amber-300 rounded-xl py-3 px-60 text-base font-bold  uppercase">yuborish</button>
                                </div>
                            </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
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
    .modal__input{
        width: 560px;
        height: 44px;
    }
    .bigbox{
        width: 1470px;
        margin: 0 auto;
    }
    .modal__box{
        height: 312px;
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

        .res__modal__text2{
            width: 196px;
            margin: 0 auto;
        }
        .res__modal__title2{
            width: 239px;
            margin: 0 auto;
            font-size: 14px;
            line-height: 18px;
            margin-block: 5px;
        }
        .modal__btn3{
            font-size: 16px;
            line-height: 16px;
        }
    }
</style>