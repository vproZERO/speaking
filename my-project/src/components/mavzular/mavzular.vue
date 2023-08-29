<template>
    <div class="bg-slate-200 p-10 bigbox">
        <h2 class="mavzular__title text-center uppercase text-3xl font-bold pt-10 mb-5">kursdagi <span class="text-blue-600">Mavzular</span></h2>
        <div class="mavzular__box flex items-start gap-5 pb-10">
            <div>
                <div class="mavzular__items flex items-center gap-2.5 bg-white rounded-lg py-3 pl-3 mb-2.5">
                    <div>
                        <img src="../../imgs/01.svg" alt="number">
                    </div>
                    <h2 class="text-base font-light">Family, Birth, Health</h2>
                </div>
                <div class="mavzular__items flex items-center gap-2.5 bg-white rounded-lg py-3 pl-3 mb-2.5">
                    <div>
                        <img src="../../imgs/02.svg" alt="number">
                    </div>
                    <h2 class="text-base font-light">Food and drinks</h2>
                </div>
                <div class="mavzular__items flex items-center gap-2.5 bg-white rounded-lg py-3 pl-3 mb-2.5">
                    <div>
                        <img src="../../imgs/03.svg" alt="number">
                    </div>
                    <h2 class="text-base font-light">Conversation</h2>
                </div>
                <div class="mavzular__items flex items-center gap-2.5 bg-white rounded-lg py-3 pl-3 mb-2.5">
                    <div>
                        <img src="../../imgs/04.svg" alt="number">
                    </div>
                    <h2 class="text-base font-light">Jobs</h2>
                </div>
                <div class="mavzular__items flex items-center gap-2.5 bg-white rounded-lg py-3 pl-3 mb-2.5">
                    <div>
                        <img src="../../imgs/05.svg" alt="number">
                    </div>
                    <h2 class="text-base font-light">Holidays</h2>
                </div>
                <div class="mavzular__items flex items-center gap-2.5 bg-white rounded-lg py-3 pl-3 mb-2.5">
                    <div>
                        <img src="../../imgs/06.svg" alt="number">
                    </div>
                    <h2 class="text-base font-light">Shops and Shopping</h2>
                </div>
                <div class="mavzular__items flex items-center gap-2.5 bg-white rounded-lg py-3 pl-3 mb-2.5">
                    <div>
                        <img src="../../imgs/07.svg" alt="number">
                    </div>
                    <h2 class="text-base font-light">Eating out</h2>
                </div>
                <div class="mavzular__items flex items-center gap-2.5 bg-white rounded-lg py-3 pl-3 mb-2.5">
                    <div>
                        <img src="../../imgs/08.svg" alt="number">
                    </div>
                    <h2 class="text-base font-light">Sports</h2>
                </div>
                <div class="mavzular__items flex items-center gap-2.5 bg-white rounded-lg py-3 pl-3 mb-2.5">
                    <div>
                        <img src="../../imgs/09.svg" alt="number">
                    </div>
                    <h2 class="text-base font-light">Music and musical instruments</h2>
                </div>
            </div>
            <div>
                <div class="mavzular__items flex items-center gap-2.5 bg-white rounded-lg py-3 pl-3 mb-2.5">
                    <div>
                        <img src="../../imgs/10.svg" alt="number">
                    </div>
                    <h2 class="text-base font-light">Countries and Nationalities</h2>
                </div>
                <div class="mavzular__items flex items-center gap-2.5 bg-white rounded-lg py-3 pl-3 mb-2.5">
                    <div>
                        <img src="../../imgs/11.svg" alt="number">
                    </div>
                    <h2 class="text-base font-light">Weather</h2>
                </div>
                <div class="mavzular__items flex items-center gap-2.5 bg-white rounded-lg py-3 pl-3 mb-2.5">
                    <div>
                        <img src="../../imgs/12.svg" alt="number">
                    </div>
                    <h2 class="text-base font-light">Everyday  verbs</h2>
                </div>
                <div class="mavzular__items flex items-center gap-2.5 bg-white rounded-lg py-3 pl-3 mb-2.5">
                    <div>
                        <img src="../../imgs/13.svg" alt="number">
                    </div>
                    <h2 class="text-base font-light">Travelling</h2>
                </div>
                <div class="mavzular__items flex items-center gap-2.5 bg-white rounded-lg py-3 pl-3 mb-2.5">
                    <div>
                        <img src="../../imgs/14.svg" alt="number">
                    </div>
                    <h2 class="text-base font-light">Culture</h2>
                </div>
                <div class="mavzular__items flex items-center gap-2.5 bg-white rounded-lg py-3 pl-3 mb-2.5">
                    <div>
                        <img src="../../imgs/15.svg" alt="number">
                    </div>
                    <h2 class="text-base font-light">Crime</h2>
                </div>
                <div class="mavzular__items flex items-center gap-2.5 bg-white rounded-lg py-3 pl-3 mb-2.5">
                    <div>
                        <img src="../../imgs/16.svg" alt="number">
                    </div>
                    <h2 class="text-base font-light">Tv Media</h2>
                </div>
                <div class="mavzular__items flex items-center gap-2.5 bg-white rounded-lg py-3 pl-3 mb-2.5">
                    <div>
                        <img src="../../imgs/17.svg" alt="number">
                    </div>
                    <h2 class="text-base font-light">Problems at home</h2>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    
}
</script>
<style scoped>
    .mavzular__box{
        width: 1216px;
        margin: 0 auto;
    }
    .mavzular__items{
        width: 598px;
        height: 48px;
    }
    .bigbox{
        width: 1470px;
        margin: 0 auto;
    }
    @media screen  and (max-width: 390px){
        .mavzular__title{
            width: 349px;
            margin: 0 auto;
            margin-block: 20px;
        }
        .mavzular__box{
            display: block;
        }
        .mavzular__items{
            width: 350px;
            margin: 0 auto;
            margin-bottom: 10px;
        }
    }
</style>