<template>
  <HelloWorld msg="Achetez une tringle à rideau personaliser"/>
  <form action="" method="get">
  <img id="img_rail" src="./assets/img/tringles-rail.jpg">

  <!-- step 1 -->
  <div class="step1" v-if="step === 'step1'">
  <h1>Etape 1/3</h1>
  <NumberInput msg=""/><br/>
   <!-- je voulais ajoutez un bouton pour valider les cm entrer dans l'input
   pour incrémenter le prix  -->
    <button type="button" class="button_step">Valider</button><br/>
    <button type="button" class="button_step" value="disable" v-on:click="step='step2'">Suivant</button>
    </div>

  <!-- step 2 -->
     <div class="step2" v-if="step === 'step2'">
  <h1>Etape 2/3</h1>
  <RadioInput msg=""/><br/>
    <button class="button_step" v-on:click="step='step3'">Valider</button>
    </div>

  <!-- step 3 -->
    <div class="step3" v-if="step === 'step3'">
  <h1>Etape 3/3</h1>
    <ColorInput msg=""/><br/>
    <button class="button_step" v-on:click="step='step1'">Ajouter au panier</button>
    </div>
<BuyInput msg="00.00€"/>
    </form>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import NumberInput from './components/NumberInput.vue'
import RadioInput from './components/RadioInput.vue'
import ColorInput from './components/ColorInput.vue'
import BuyInput from './components/BuyInput.vue'


export default {
  name: 'App',
  components: {
    HelloWorld,
    NumberInput,
    RadioInput,
    ColorInput,
    BuyInput,
  },
  data(){
    return{
    step: 'step1',
    }
  }
}


</script>

<style>
.button_step{
  padding: 5%;
  background-color:#0c1251;
  color: white;
}
.button_step:hover{
  background-color:#0c1251;
  cursor: pointer;
}
form{
  display:flex;
}
.step1{
  margin-left: 20%;
}
.step2{
  margin-left: 10%;
}
.step3{
  margin-left: 10%;
}
#img_rail{
  display: flex;
  height: 525px;
  margin-left: 10%;
}
#img_rail:hover{
  cursor: pointer;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
