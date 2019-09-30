<template>
  <div>
    <navbar/>
    <div class="corporate">
      <div class="columns">
        <div class="column is-two-fifths">
          <h1>Corporate Service</h1>
          <br>
          <p>Eudeka! menyediakan berbagai layanan untuk perusahaan Anda. Layanan yang kami berikan berfokus kepada solusi teknis dari permasalahan bisnis yang ada di perusahaan.</p>
          <br>
         <b-button type="info" @click="student">Kontak Kami</b-button>
        </div>
      </div>
    </div>

    <div class="content-section">
      <div class="columns">
        <div class="column is-half">
          <img src="@/assets/image/corporate1.jpg" alt="">
        </div>
        <div class="column">
          <h1>Corporate Training</h1>
          <br>
          <h3>Eudeka! akan membantu perusahaan Anda untuk dapat meningkatkan kemampuan teknis personal timnya.</h3>
          <br>
          <br>
          <h3>Kami menyediakan training Android, iOS, Flutter, NodeJS, VueJS, Kubernetes, Docker, dan .NET Core. Kami siap untuk menyesuaikan silabus dengan kebutuhan materi di perusahaan Anda bekerja.</h3>
          <br>
          <br>
          <h3>Training dapat dilakukan di tempat Anda atau di training center kami di Bandung.</h3>
          <br>
          <br>
          <b-button type="info" @click="student">Kirim Inquiry</b-button>
        </div>
      </div>
      <div class="columns">
        <div class="column is-half">
          <h1>Apps Review & Suggestion</h1>
          <br>
          <h3>Kami dapat melakukan review dan memberikan masukan terhadap aplikasi mobile yang telah dibuat oleh Anda atau vendor Anda.</h3>
          <br>
          <br>
          <h3>Kami memberikan masukan secara detail baik dari sisi keamanan, performa, coding style, dan UI dan UX.</h3>
          <br>
          <br>
          <h3>Kami dapat memberikan solusi jika terdapat masalah yang di aplikasi yang sudah dibuat, seperti bagaimana membuat ukuran aplikasi yang lebih kecil maupun bagaimana memproteksi aplikasi Anda agar aman dari pihak yang tidak bertanggung-jawab.</h3>
          <br>
          <br>
          <b-button type="info" @click="student">Kirim Inquiry</b-button>
        </div>
        <div class="column">
          <img src="@/assets/image/corporate2.jpg" width="100%" alt="">
        </div>
      </div>
      <div class="columns">
        <div class="column is-half">
          <img src="@/assets/image/corporate3.jpg" width="100%" alt="">
        </div>
        <div class="column">
          <h1>Technical Expert Consulting</h1>
          <br>
          <h3>Kami bekerjasama dengan para expert di bidang teknologi mobile, website, backend, dan desain untuk membantu Anda dalam menyelesaikan masalah atau mendesain arsitektur aplikasi yang Anda buat.</h3>
          <br>
          <br>
          <h3>Kami dapat hadir ke tempat Anda untuk memberikan konsultasi serta dapat melakukan pendampingan agar solusi yang kami berikan dapat diimplementasi dengan baik.</h3>
          <br>
          <br>
          <b-button type="info" @click="student">Kirim Inquiry</b-button>
        </div>
      </div>
    </div>
    <hr>
    <foot/>


  </div>
</template>

<script>
  import Navbar from '@/components/Homepage/navbar.vue'
  import Foot from '@/components/Homepage/footer.vue'
  export default {
    name: 'Corporate',
    components: {
      Navbar,
      Foot
    }
    
  }
</script>

<style scoped>
  .button {
    margin-left: 50px;
  }
  .service {
    margin: 0 0 0 10%;
    background: white;
    width: 40%;
    height: 250px;
  }
  .corporate {
    background: url('../../assets/image/corp.jpg');
    background-size: cover;
    background-position: center;
    background-attachment: fixed;
    width: 100%;
    height: 500px;
    margin: 0 0 0 0;
  }
  .columns {
    padding: 8% 0 0 0;
    margin: 0 0 0 10%;

  }
  h1 {
    font-size: 50px;
    line-height: 60px;
  }
  .content-section {
    margin: 0 10% 0 10%;
  }
  p {
    font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
    font-size: 20px;
    font-weight: 500;
    font-style: oblique;
  }
</style>