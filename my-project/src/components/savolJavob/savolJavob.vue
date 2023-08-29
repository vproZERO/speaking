<template >
    <div class="bg-slate-200 p-10 bigbox">
        <h2 class="savollar__title uppercase text-center font-bold text-3xl pt-10 mb-5">Savol & <span class="text-blue-600">Javoblar</span></h2>
        <div class="savol__box flex  gap-14  mx-auto mb-2.5">
            <div>
                <div class="savol__accordion mt-5 overflow-hidden">
                    <Accordion class="accordion__box bg-white py-3 pl-3 pr-3 rounded-lg text-base font-bold mb-5" :number="1" :title="`149 000 so‘m kursning umumiy narximi?`">
                        <p class="respons__text text-sm font-normal mt-5">Ha, 149 ming to‘lovdan so‘ng boshqa to‘lov yo‘q darslarni o‘rganishni boshlaysiz.</p>
                    </Accordion>
                    <Accordion class="accordion__box bg-white py-3 pl-3 pr-3 rounded-lg text-base font-bold mb-5" :number="2" :title="`Darslar qachon boshlanadi?`">
                        <p class="respons__text text-sm font-normal mt-5">To’lovdan so’ng sizni yopiq guruhga qo’shishadi va guruhda dars boshlanish sanasi e’lon qilinadi</p>
                    </Accordion>
                    <Accordion class="accordion__box bg-white py-3 pl-3 pr-3 rounded-lg text-base font-bold mb-5" :number="3" :title="`Darsga kira olmasam darsdan qolib ketamanmi?`">
                        <p class="respons__text text-sm font-normal mt-5">Yo’q, agar darsga qatnasha olmasangiz, darsdan so’ng guruhingizga zoom zapisi tashlab beriladi.</p>
                    </Accordion>
                    <Accordion class="accordion__box bg-white py-3 pl-3 pr-3 rounded-lg text-base font-bold mb-5" :number="4" :title="`Uyga vazifalar ham bo’ladimi?`">
                        <p class="respons__text text-sm font-normal mt-5">Ha, uyga vazifalar beriladi va kuratorlar tomonidan tekshiriladi.</p>
                    </Accordion>
                    <Accordion class="accordion__box bg-white py-3 pl-3 pr-3 rounded-lg text-base font-bold mb-5" :number="5" :title="`Bu kursda qatnashish uchun qanday darajaga ega bo’lish kerak?`">
                        <p class="respons__text text-sm font-normal mt-5">0 dan intermediate levelgacha bo’lganlar uchun to’g’ri keladi. Starter dan elementary darajasigacha bo’lganlar uchun alohida guruh, pre-intermediate dan intermediate darajasigacha biladiganlar uchun alohida guruh ochiladi.</p>
                    </Accordion>
                    <Accordion class="accordion__box bg-white py-3 pl-3 pr-3 rounded-lg text-base font-bold mb-5" :number="6" :title="`O’z darajamni qanday bilsam bo’ladi?`">
                        <p class="respons__text text-sm font-normal mt-5">Sotuvchilarimizga aloqaga chiqsangiz qisqa savol-javob orqali darajangizni bilib olishingiz mumkin.</p>
                    </Accordion>
                    
                </div>
                <div class="mb-20 w-80 mx-auto pb-5">
                    <button v-on:click="isOpen = !isOpen" class="respons__btn uppercase bg-amber-300 hover:bg-amber-200 rounded-lg py-3 px-5 text-base font-bold">chegirmada sotib olish</button>
                    
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
            <div class="savollar__big_img">
                <img src="../../imgs/big_img.svg" alt="img">
            </div>
        </div>
        
    </div>
</template>
<script>
import Accordion from '../accordion/accordion.vue'
export default {
    components: {
        Accordion,
    },
    data : () => {
        return {
            isOpen : false,
            onOpen : false
        }
    }
    
}
</script>
<style scoped>
    .savol__box{
        width: 1222px;
    }
    .savollar__big_img{
        margin-top: -130px;
    }
    .savol__content{
        width: 807px;
    }
    .accordion__box{
        width: 807px;
    }
    .savol__accordion{
        height: 472px;
    }
    .kursga__tolov__btn{
        width: 600px;
        height: 351px;
    }
    .modal{
        width: 600px;
    }
    .modal__input{
        width: 560px;
        height: 44px;
    }
    .bigbox{
        width: 1470px;
        margin: 0 auto;
    }
    @media screen and (max-width: 390px){
        .savollar__title{
            width: 349px;
            margin: 0 auto;
            margin-block: 20px;
            font-size: 24px;
            line-height: 32px;
        }
        .savol__box{
            width: 350px;
            margin: 0 auto;
            display: block;
        }
        .savol__accordion{
            width: 350px;
            height: 526px;
            margin-bottom: 20px;
        }
        .accordion__box{
            width: 350px;
            font-size: 16px;
            line-height: 24px;
        }
        .respons__text{
            width: 330px;
            font-size: 14px;
            line-height: 20px;
        }
        .respons__btn{
            width: 300px;
            padding: 12px 21px;
            font-size: 16px;
            line-height: 24px;
            margin: 0 auto;
        }
        .savollar__big_img{
            width: 256px;
            height: 340px;
            margin: 0 auto;
            margin-bottom: -50%;
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