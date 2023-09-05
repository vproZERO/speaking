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
                    <Modal :class="isOpen ? 'block' : 'hidden'"   class=" bg-black bg-opacity-25 fixed inset-0 z-50 mx-auto "/>
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
import Modal from '../modal/modal.vue'
export default {
    components: {
        Accordion,
        Modal
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
    }
</style>