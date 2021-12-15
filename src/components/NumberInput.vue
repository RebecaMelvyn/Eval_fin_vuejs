<template>
  <div class="hello">
  <!-- input type number de la step 1 -->

  <label>Longueur du rail</label><br/>
    <input placeholder="min. 0 cm / max. 200 cm" type="number"
    id="input" max="200" inputmode="numeric" required />

  </div>
</template>

<script>
export default {
  name: 'NumberInput',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#title{
  margin-bottom: 5%;
}
label{
    font-weight: bold;
}
input{
    margin-top: 5px;
    padding-right: 30px;
    padding-left: 40px;
    padding-top: 10px;
    padding-bottom: 10px;
    border: solid 1px;
    text-align: justify;
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
