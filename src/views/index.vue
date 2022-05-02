<template>
  <h1>Index</h1>
  <div class="d-grid gap-2">
  <button class="btn btn-primary" type="button" @click="clickclick()">กดเลย</button>
  </div>
</template>
<script>
//import section

//export section
export default {
  name : 'index',
  components : {

  },
  data() {
    return {
      checked: true,
    }
  },
  methods : {
    clickclick : function(){
      if(this.checked !== false) this.$router.push('/test')
    }
  },
}
</script>
<style>
</style>