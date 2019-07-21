<template>
  <div class="hello">
    <input type="text" id="owen" v-model.number="number">
    <div v-for="num in number" :key="num">
        <count @addle="handeladdle" @deeple="handeldeeple"></count>
    </div>
    <div><h1>{{sum}}</h1></div>
  </div>
</template>

<script>
import count from './frist.vue'
export default {
  name: 'last-vue',
  components:{count},
  data(){
        return{
          number:0,
          sum:0
        }
  },
  methods:{
      handeladdle:function(){
        this.sum ++;
      },
      handeldeeple:function(){
        this.sum --;
      }
  },
  watch:{
    number:function(){
      this.sum = 0
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
