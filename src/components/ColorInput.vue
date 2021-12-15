<template>
  <div class="hello">
<!-- input type radio de la step 3 -->

<input type="radio" name="color-type" class="radio" id="color-type-a" checked>
<label for="color-type-a">
<div class="bloc black"></div>
<h4>Noir</h4>
</label>

<input type="radio" name="color-type" class="radio" id="color-type-b" >
<label for="color-type-b">
<div class="bloc white"></div>
<h4>Blanc</h4>
</label>
<br>

  </div>
</template>

<script>
export default {
  name: 'RadioInput',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.img_radio{
    width: 100px;
}
.bloc{
    height: 50px;
    width: 200px;
}
.black{
    background-color: black;
}
.white{
    background-color: white;
}

/*CSS pour les input radio de l'étape n°3 */

input[type="radio"].radio {
  display: none;
  margin-top: 5%;
  flex-wrap: wrap;
  width: 50%w;
}
input[type="radio"].radio + label {
  padding: 5%;
  padding-left: 25px;
  padding-right: 25px;
  border: 1px solid #e7f5f9;
}
input[type="radio"].radio:checked + label {
  border: 1px solid #000;
  background: #e7f5f9;
  
}
input[type="radio"].radio:hover + label {
  cursor: pointer;
}

.hello{
    display: flex;
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
