<template>
  <div>
    <navbar/>
    <div class="event">
      <div class="columns">
        <div class="column">
          <h1>Workshop Artifical Intelligence</h1>
        </div>
      </div>
      <div class="columns description">
        <div class="column">
          <p>This Workshop is aimed to any people who having interesting in artificial Intelligenc. This event will be held in main auditorium FMIPA unri</p>
          <h1>Cooming Soon !!!!</h1>
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
    name: 'Event',
    components: {
      Navbar,
      Foot
    }
    
  }
</script>

<style lang="scss" scoped>
  .event {
    margin: 5% 0 0 0;
  }
  .columns {
    text-align: center;
  }
  h1 {
    font-size: 50px;
  }
  .description {
    font-size: 20px;
    font-weight: 400;
    margin: 0 15% 0 15%;

  }
</style>