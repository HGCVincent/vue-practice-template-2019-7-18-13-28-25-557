<template>
  <div class="hello">
    <button v-on:click="desc"> - </button>
    <span>{{count}}</span>
    <button v-on:click="asc"> + </button>
  </div>

</template>

<script>

    export default {
        name : "helloVue",
        data(){
            return {
                count :0
            }
        },
        methods:{
            desc(){
                this.count --
            },
            asc(){
                this.count ++
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
