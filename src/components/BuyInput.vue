<template>
  <div class="hello">
    <div id="price">
    <a>{{ msg }}</a>
    </div>
  </div>
</template>

<script>
export default {
  name: 'BuyInput',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#price{
    width: 15em;
    height: 5%;
    padding: 5%;
    background-color:#e7f5f9;
    margin-top: 22em;
}

#title{
  margin-bottom: 5%;
}

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
