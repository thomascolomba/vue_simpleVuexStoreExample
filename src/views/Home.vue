<template>
  <div class="home">
    {{val}}
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
  }
}
</script>
