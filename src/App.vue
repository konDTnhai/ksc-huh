<template>
  <div id="app">
    <router-view v-slot="{ Component }">
    <component :is="Component"></component>
    </router-view>
  </div>
</template>

<script>
//import section

//export section
export default {
  name: 'App',
  data() {
    return {

    }
  },
  methods : {

  },
  //beforeCreate hook สำหรับการตรวจสอบและ Init
  beforeCreate() {
    window.liff.init({ liffId : ""})
    .then(() => {
      if(!window.liff.isInClient()){
        if(!window.liff.isLoggedIn()){
          window.liff.login()
        }
      }
    })
  },
}
</script>

<style>
#app {
  font-family: sarabun;
  color: #2c3e50;
  margin: 15px;
}
</style>
