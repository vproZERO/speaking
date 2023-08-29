<template>
    <div class="bg-blue-600 p-10 bigbox">
        <h2 class="kutmoqda__title text-center text-3xl font-bold uppercase pt-10 mb-9 text-white">kursda sizni <span class="text-amber-300">nimalar kutmoqda?</span></h2>
        <div class="kutmoqda_respons__box hidden relative bg-white flex p-5 rounded-xl justify-between">
            <div>
                <h2 class="text-2xl font-bold uppercase w-44">kursda sizni <span class="text-blue-600">nimalar kutmoqda?</span></h2>
            </div>
            <div class="respons__img absolute bottom-0 right-0">
                <img src="../../imgs/tutor2.svg" alt="tutor">
            </div>
        </div>
                <div class="respons__box flex justify-between">
                    <div class="flex items-center gap-4 mb-5 nimalar__miniBox">
                        <div>
                            <img src="../../imgs/noutbook.svg" alt="noutbook">
                        </div>
                        <h2 class="text-lg font-bold text-white nimalar__text">Haftada 3 kun zoom orqali darslar</h2>
                    </div>
                    <div class="flex items-center gap-4 mb-5 nimalar__miniBox">
                        <h2 class="text-lg font-bold text-right text-white nimalar__text">Darsda qatnasha olmasa, zapislar tashlab beriladi</h2>
                        <div>
                            <img src="../../imgs/rec.svg" alt="recording">
                        </div>
                    </div>
                </div>
                <div class="flex justify-between respons__box">
                    
                    <div class="flex items-center gap-4 mb-5 nimalar__miniBox">
                        <div>
                            <img src="../../imgs/sms.svg" alt="sms">
                        </div>
                        <h2 class="text-lg font-bold text-white nimalar__text">Kuratorlar nazoratida savol-javoblar</h2>
                    </div>
                    <div class="flex items-center gap-4 mb-5 nimalar__miniBox">
                        <h2 class="text-lg text-right font-bold text-white nimalar__text">Uyga vazifalar bajarilishi nazorati</h2>
                        <div>
                            <img src="../../imgs/vazifa.svg" alt="homework">
                        </div>
                        
                    </div>
                    
                </div>
                <div class="respons__box mb-10 ">
                    <div class="nimalar__miniBox flex items-center gap-4 mb-5">
                        <div>
                            <img src="../../imgs/certificate.svg" alt="certificate">
                        </div>
                        <h2 class="text-lg font-bold text-white nimalar__text">Kursni tugatgach sertifikat bilan taqdirlanadi</h2>
                    </div>
                    <div class="respons__button hidden mb-20">
                        <button v-on:click="isOpen = !isOpen" class="uppercase text-base font-bold bg-amber-300 rounded-lg py-3 px-3 hover:bg-amber-200">Chegirmada sotib olish</button>
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
            onOpen : false
        }
    }
}
</script>
<style scoped>
    .nimalar__box{
        width: 1216px;
        margin: 0 auto;
    }
    .modal__input{
        width: 560px;
        height: 44px;
    }
    .kutmoqda_respons__box{
        width: 350px;
        margin: 0 auto;
    }
    .respons__img{
        width: 161px;
        height: 172px;
    }
    .nimalar__miniBox{
        width: 598px;
    }
    .nimalar__text{
        width: 432px;
    }
    .bigbox{
        width: 1470px;
        margin: 0 auto;
    }
    .respons__button{
        width: 250px;
        margin: 0 auto;
    }
    .modal__box{
        height: 312px;
    }
    @media screen and (max-width: 390px){
        .kutmoqda__title{
            display: none;
        }
        .kutmoqda_respons__box{
            display: block;
            margin-block: 20px;
        }
        .nimalar__box{
            display: block;
        }
        .nimalar__miniBox{
            width: 350px;
            margin: - auto;
        }
        .respons__box{
            display: block;
            margin: 0 auto;
            width: 350px;
        }
        .respons__button{
            display: block;
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