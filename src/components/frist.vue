<template>
  <div class="hello">
    <button @click="add">+</button>
    <span>{{ count }}</span>
    <button @click="deep">-</button>
    {{data}}
  </div>
</template>

<script>
export default {
  name: 'count',
  data(){
      return {
          count :0
      }
  },
  methods:{
      add(){
         this.count++
         this.$emit("addle")
      },
      deep(){
         this.count--
         this.$emit("deeple")
      }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
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
