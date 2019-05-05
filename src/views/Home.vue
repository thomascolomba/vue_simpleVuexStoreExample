<template>
  <div class="home">
    <p>This a value from the Vuex store :<p/>
    <span style="font-weight:bold;">{{val}}</span>
    <p>Please go to the About page to edit it.</p>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'home',
  data: function () {
    return {
      val: this.$store.state.myVar
    }
  },
  created () {
    this.val = this.$store.state.myVar
  }
}
</script>
