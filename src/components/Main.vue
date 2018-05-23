<template>
  <div>{{this.value}}</div>
</template>

<script>
import Tsp from '@/assets/Tsp'

export default {
  name: 'Main',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  computed: {
    value () {
      const t = new Tsp()
      return t.hello()
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
