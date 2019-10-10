<template>
  <div>
    <navbar/>
    <background/>
    <ongoing/>
    <category/>
    <meet/>
    <foot/>
  </div>
</template>

<script>
// @ is an alias to /src
import Background from '@/components/Homepage/background.vue'
import Navbar from '@/components/Homepage/navbar.vue'
import Category from '@/components/Homepage/sectionResearchCategory.vue'
// import Profile from '@/components/Homepage/profile.vue'
import Ongoing from '@/components/Homepage/sectionOngoingResearch.vue'
import Foot from '@/components/Homepage/footer.vue'
import Meet from '@/components/Homepage/meetSupporter.vue'

export default {
  name: 'home',
  components: {
    Navbar,
    Background,
    Category,
    Ongoing,
    Meet,
    Foot
  },
  data () {
    return {
      
    }
  },
  methods: {

  }
}
</script>
<style scoped>

</style>