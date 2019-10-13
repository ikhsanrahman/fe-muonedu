<template>
  <div>
    <div class="ongoing">
      <div class="title">
        <h1>Sedang dibuka!</h1>
        <div class="columns">
          <div class="column">
            <h2>Kelas Python From Zero to Hero</h2>
            <h4>Daftar Sekarang dan Kelas akan dimulai pada bulan November 2019</h4>
          </div>
          <div class="column is-two-thirds">
          <b-button  type="is-info" @click="python">Info Lengkap
            <b-icon
              icon="arrow-right-circle"
              size="is-small">
            </b-icon>
          </b-button>
          </div>
        </div>
      </div>
    </div>

  </div>
</template>

<script>
  export default {
    data () {
      return {
        
      }
    },
    methods: {
      python () {
        this.$router.push('/student')
      }
    }
  }
</script>

<style scoped>
.columns {
  padding: 10px 20px 30px 11.5%;
  margin: 10px 0 0 0;
}
.column h2 {
  font-size: 26px;
}
.is-two-thirds {
  padding: 30px 0 0 30%;
}
.is-one-quarter {
  padding: 30px;
}
.title {
  padding: 50px 0 0 0;
}
.title h1 {
  font-weight: bolder;
  font-size: 40px;
  margin-left: 12%;
}
.title h3 {
  text-align: center;
  font-style: oblique;
  font-weight: 300;
  padding: 20px 0 0 0;
  font-size: 20px;
}
.ongoing {
  /* background: url('../../assets/image/blueBackground.jpg') no-repeat; */
  background-size: cover;
  background-position: center;
  background-attachment: fixed;
  height: 100%; 
}

</style>