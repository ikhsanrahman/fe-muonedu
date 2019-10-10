<template>
  <div>
    <navbar/>
    <div class="student">
      <div class="columns" style="margin: 0 20% 15px 20%">
        <div class="column" style="padding:5% 0 0 0;">
          Oktober bulannya belajar !!
          <br>
          <br>
          Ada beberapa Pilihan Program yang bisa kamu ikuti. kamu juga bisa memilih metode pelatihan secara intensif, kelompok bahkan private.
          <br>
          <br>
          Jangan menaruh harapan sama doi yang gapeka sama kode kamu, mulai sekarang taruh harapan yang cerah dengan belajar koding di Muonedu! Yuk, daftar sekarang juga!
          <br>
          <br>
          <br>
          <b-button type="info" style='margin:0 0 20px 30%;' @click="student">Daftar Sekarang</b-button>
        </div>
        <div class="column">
          <img src="@/assets/image/python.png" style="padding: 10% 0 5% 10%" alt="">
        </div>

      </div>
    </div>
    <price/>
  </div>
</template>

<script>
  import Navbar from '@/components/Homepage/navbar.vue'
  import Price from '@/views/Price/price.vue'

  export default {
    name: 'student',
    components: {
      Navbar,
      Price
    },
    data () {
      return {

      }
    }
    
  }
</script>

<style scoped>
  .student {
    background: rgb(255, 230, 97);
  }
</style>