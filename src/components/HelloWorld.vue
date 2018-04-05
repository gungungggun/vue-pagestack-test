<template lang="pug">
  div.stack
    div(v-for="page in pages")
      component(:is="page")
</template>

<script lang="coffee">
import Page1 from '@/components/Page1.vue'
import Page2 from '@/components/Page2.vue'
import Page3 from '@/components/Page3.vue'
import Page4 from '@/components/Page4.vue'
import Page5 from '@/components/Page5.vue'

export default {
  name: 'HelloWorld',
  data: () ->
    pages: [
      Page1
      Page2
      Page3
      Page4
      Page5
    ]
}
</script>

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
