
<script>

  export default {
    data: ()=>({
      contador:10,
    }),

    methods:{
      saludar(){
        console.log("Hola Guapeton")
      },
      incrementar(){
        this.contador=this.contador+1
      },
      disminuir(){
        this.contador=this.contador-1
      },
      resetear(){
        this.contador=10;
      },
    }
  };

</script>



<template>
  <!--
    <nav class="navbar navbar-light bg-light fixed-top">
  <span class="navbar-brand mb-0 h1">Milton Jair Rubio Juárez DMI 10 A </span>
  </nav>
-->
  <img src="./assets/logo.svg" alt="Logo VUE" width=" 125" height="125" class="fixed">


  <container>
  <small> <h1> Hola desde VUE.js  </h1></small>
 
  <hr>
  <h2>Contador desde {{contador}}</h2>
  <button @click="incrementar()">+1</button>
  <button @click="disminuir()">-1</button>
  <button @click="resetear()">Reset</button>
  

</container>

</template>

<style scoped> 
h1{
  font-weight: bolder;
  
}
nav{
margin-top: 0;
padding-top: 0;
}

.container{
  text-align: center;
}
  

  small{
    color: #666;
  }

  h2{
    font-size:2.5rem;

  }

  button{
    cursor:pointer;
    font-size: 1.5rem;
    margin:0px 8px;

  }
</style>