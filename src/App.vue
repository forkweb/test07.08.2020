<template>
  <div id="app">
    <div class="section_app">
      <div class="container">
        <ListNote msg="Welcome to Your Vue.js App"/>
      </div>
    </div>
  </div>
</template>

<script>
import ListNote from './components/ListNote.vue'

export default {
  name: 'App',
  components: {
    ListNote
  }
}
</script>

<style lang="scss" type="text/scss">
  @import "~@/style/app.scss";
</style>
