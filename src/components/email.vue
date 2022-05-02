<template>
  <p>Emailcustom</p>
  <ul id="email" v-for="user in users"> 
  <li >
    {{ user.name }}
  </li>
  <li >
    {{ user.email }}
  </li>
</ul>
</template>

<script>
//import section

//export section
export default {
  name : 'email',
  components : {

  },
  props : {

  },
  data() {
    return {
      users : [
        {
          name :"kittisarn",
          email : 'chewjinda99@gmail.com',
        },
        {
          name :"kitti",
          email : 'chewjinda94@gmail.com',
        },
        {
          name :"sarn",
          email : 'chewjinda96@gmail.com',
        },
        {
          name :"kit",
          email : 'chewjinda95@gmail.com',
        },
      ],
    }
  },
  methods : {

  },
}
</script>

<style>
</style>