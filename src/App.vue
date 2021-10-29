<template>
  <div id="app">

    <h1 class="__title">Welcome to <div class="__zerops">ZEROPS</div> recipe including <div class="__tech">Vue.js</div> technology</h1>

    <div class="__checklist">

      <h3 class="__checklist-title"><strong>Your next steps?</strong></h3>

      <div class="__checklist-item">
        <md-checkbox v-model="array" value="1"></md-checkbox>
        Fork repository
      </div>

      <div class="__checklist-item">
        <md-checkbox v-model="array" value="2"></md-checkbox>
        Open build and deploy settings and connect
      </div>

      <div class="__checklist-item">
        <md-checkbox v-model="array" value="3"></md-checkbox>
        Push a new commit
      </div>

    </div>

  </div>
</template>

<script>

// import { MdCheckbox } from 'vue-material/dist/components'
import 'vue-material/dist/vue-material.min.css'
import 'vue-material/dist/theme/default.css'

export default {
  name: 'App',
  data: () => ({
    array: []
  })
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
.__title {
  display: block;
  width: 100%;
  max-width: 800px;
  margin: 0 auto;
  padding: 72px;
  font-size: 45px;
  line-height: 80px;
  font-family: monospace;
  text-align: center;
}

.__zerops {
  display: inline-block;
  color: #00b1a3;
}

.__tech {
  display: inline-block;
  color: #00b1a3bf;
}

.__checklist {
  max-width: 410px;
  margin: 0 auto;
  margin-top: 48px;
  padding: 24px;
  background: #fff;
  border-radius: 8px;
  text-align: left;
}

.__checklist-item {
  margin-bottom: 12px;
}

.__checklist-item .md-checkbox {
  margin: 0;
  margin-right: 4px;
  vertical-align: bottom;
}
</style>
