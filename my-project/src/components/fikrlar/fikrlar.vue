<template >
    <div class="bg-amber-300 p-10 bigbox">
        <h2 class="fikrlar__title uppercase text-center pt-10 pb-5 font-bold text-3xl "><span class="text-blue-600">kurs bitiruvchilarning </span> fikrlari</h2>
        <div class="fikrlar__Box flex items-center gap-2.5 pb-10">
            <div class=" flex gap-2.5 mb-2.5">
                <div>
                    <img src="../../imgs/fikrlar1.svg" alt="img">
                </div>
                <div>
                    <img src="../../imgs/fikrlar2.svg" alt="img">
                </div>
            </div>
            <div class="flex gap-2.5">
                <div>
                    <img src="../../imgs/fikrlar3.svg" alt="img">
                </div>
                <div>
                    <img src="../../imgs/fikrlar4.svg" alt="img">
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
    .fikrlar__Box{
        width: 710px;
        margin: 0 auto;
    }
    .bigbox{
        width: 1470px;
        margin: 0 auto;
    }
    @media screen and (max-width: 390px){
        .fikrlar__title{
            width: 349px;
            font-size: 24px;
            line-height: 32px;
            margin: 0 auto;
        }
        .fikrlar__Box{
            display: block;
            margin: 0 auto;
            width: 350px;
        }
    }
</style>