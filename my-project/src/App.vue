<template>
  <div >
      <Header/>
    <div>

      <KimlarUchun/>
      <NimalarKutmoqda/>
      <Mavzular/>
      <Fikrlar/>
      <SavolJavob/>
      <Footer/>
    </div>
  </div>
</template>
<script>
import Header from './components/header/header.vue'
import KimlarUchun from './components/kimlaruchun/kimlaruchun.vue'
import NimalarKutmoqda from './components/nimalarkutmoqda/nimalarkutmoqda.vue'
import Mavzular from './components/mavzular/mavzular.vue'
import Fikrlar from './components/fikrlar/fikrlar.vue'
import SavolJavob from './components/savolJavob/savolJavob.vue'
import Footer from './components/footer/footer.vue'
export default {
  components : {
    Header,
    KimlarUchun,
    NimalarKutmoqda,
    Mavzular,
    Fikrlar,
    SavolJavob,
    Footer,
  }
}
</script>
<style >
</style>