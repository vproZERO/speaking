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
                        <Modal :class="isOpen ? 'block' : 'hidden'"   class=" bg-black bg-opacity-25 fixed inset-0 z-50 mx-auto "/>
                
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
    }
</style>