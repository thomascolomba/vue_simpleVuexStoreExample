<template>
  <div class="about">
    <h1>This is the about page</h1>
    <p>Fill a value to be stored in Vuex store and displayed in page Home :</p>
    <input type="text" v-model="valueToStore" @change="valueToStoreChange"/>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'home',
  data: function () {
    return {
      valueToStore: ''
    }
  },
  methods: {
    valueToStoreChange: function () {
      this.$store.state.myVar = this.valueToStore
    }
  },
  created () {
    this.valueToStore = this.$store.state.myVar
  }
}
</script>
