<template>
  <div class="hello">
<!-- input type radio de la step 2 -->

<input type="radio" name="rail-type" class="radio" id="rail-type-a" checked>
<label for="rail-type-a">
<img class="img_radio" src="../assets/img/radio_1.jpg">
<h4>Modèle DS : Fixation au <br/>plafond pour rideaux légers </h4>
<h5>(sans doublure, hauteur max 300cm)</h5>
</label>

<input type="radio" name="rail-type" class="radio" id="rail-type-b" >
<label for="rail-type-b">
<img class="img_radio" src="../assets/img/radio_2.png">
<h4>Modèle CS : Fixation au <br/>plafond ou au mur pour<br/>
rideaux lourds </h4>
<h5>(doublé, hauteur + 300cm)</h5>
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

#title{
  margin-bottom: 5%;
}
/*CSS pour les input radio de l'étape n°2 */

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
