<template>
  <div class="translate">
    <h1>{{ msg }}</h1>
    <input type="text" v-model="Name">
    <button @click="searchName">translate</button>
    {{SearchResult}}
  </div>
</template>

<script>
import axios from 'axios'
export default {
  name: 'translate',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      Name: '私は東京へ行きたい。',
      SearchResult: []
    }
  },
  methods: {
    async searchName () {
      const resp = await axios.get(encodeURI('https://translate.altair626.work?ja_text=' + this.Name))
      this.SearchResult = resp.data.message
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