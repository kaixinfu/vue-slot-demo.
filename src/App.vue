<template>
  <div id="app">
    <Demo :tree="tree" />
  </div>
</template>

<script>
import Demo from './demo'

export default {
  name: 'App',
  components: {
    Demo
  },
  data() {
    return {
      tree: {
        name: 'AA',
        key: 'a1',
        children: [
            {name: 'BB', key: 'b1',
                children: [
                    {name: 'CC', key: 'c1'},
                    {name: 'CC', key: 'c2'}
                ]
            }
        ]
      }
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
