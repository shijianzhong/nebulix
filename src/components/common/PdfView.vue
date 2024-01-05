<template>
   <div class="pdf_container">
      <iframe
        :src="`pdf/web/viewer.html?file=${pdfUrl}`"
        class="pdf-window"
        width="100%"
        height="100%"
        frameborder="0"
      ></iframe>
    </div>
</template>
  
<script setup>
import {ref} from "vue"
const pdfUrl = ref("../jianying.pdf")


</script>
<style scoped>
.pdf_container{
  width: 100%;
  height: 1000px;
}
iframe{
    width: 100%;
    height: 100%;
}
</style>