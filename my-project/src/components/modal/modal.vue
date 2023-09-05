<template>
    <div>
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
    .modal__box{
        height: 312px;
    }
    .modal__input{
        width: 560px;
        height: 44px;
    }
    @media screen and (max-width: 390px){
        .modal__box{
            width: 350px;
            height: 300px;
            margin: 0 auto;
            padding: 10px;
            margin-bottom: 40px;
        }
        .kursga__tolov__btn{
            margin-top: 5px;
        }
        .modal__input{
            width: 310px;
            height: 25px;
            padding: 3px ;
            margin-bottom: 5px;
        }
        .modal__btn{
            width: 310px;
            height: 44px;
            padding: 12px 114px;
        }
        .modal__btn2{
            width: 310px;
            height: 25px;
            padding: 0 ;
            font-size: 12px;
            line-height: 18px;
        }
        .res__modal__title{
            width: 233px;
            font-size: 14px;
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
            font-size: 12px;
            line-height: 18px;
            
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