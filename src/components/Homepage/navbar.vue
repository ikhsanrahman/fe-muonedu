<template>
  <div>
      <b-navbar fixed-top >
        <template slot="brand">
          <img class="logo" @click='home'
            src="https://cdn5.f-cdn.com/contestentries/908047/20897340/585714544243e_thumb900.jpg"
            alt="Photonic Research Center of Riau">
        </template>
<!--         <template slot="start">
          <b-navbar-item>
            <a @click="cooperation">
              Cooperation
            </a>
          </b-navbar-item>
          <b-navbar-dropdown label="Info">
            <b-navbar-item>
              <a @click="contact">
                Contact
              </a>
            </b-navbar-item>
            <b-navbar-item>
              <a @click="event">
                Event
              </a>
            </b-navbar-item>
          </b-navbar-dropdown>
        </template> -->

        <template slot="end">
          <b-navbar-item>
            <a @click="home">
              Home
            </a>
          </b-navbar-item>
          <b-navbar-item>
            <a @click="corporate">
              Corporate
            </a>
          </b-navbar-item>
          <b-navbar-item>
            <a @click="contact">
              Contact Us
            </a>
          </b-navbar-item>
          <b-navbar-item>
            <a @click="event">
              Event
            </a>
          </b-navbar-item>
        </template>
      </b-navbar>
      <manage-login-dialog :dialog.sync="dialogLogin"></manage-login-dialog>
      <manage-register-dialog :dialog.sync="dialogSignup"></manage-register-dialog>
  </div>
</template>

<script>
import ManageLoginDialog from '@/components/Dialog/manageLoginDialog.vue'
import ManageRegisterDialog from '@/components/Dialog/manageRegisterDialog.vue'


export default {
  components: {
    'manage-login-dialog': ManageLoginDialog,
    'manage-register-dialog': ManageRegisterDialog
  },
  data () {
    return {
      dialogLogin: false,
      dialogSignup: false,
      agileShow: true

    }
  },
  created () {

  },
  methods: {
    home () {
      this.$router.push({path:'/'})
    },
    corporate () {
      this.$router.push({name:'corporate'})

    },
    contact () {
      this.$router.push({name:'contact'})
      
    },
    event () {
      this.$router.push({name:'event'})
      
    }

  }
    
}
</script>

<style scoped>
 
  .navbar {
    box-shadow: 2px 2px rgb(215, 218, 214);
  }
  .logo {
    width: 200px;
    height: 80px;
    cursor: pointer;
  }
  .navbar-item {
    width: 60%;
    text-align: center;
  }
</style>