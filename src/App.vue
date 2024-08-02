<template>
<div>
     <div class="input-field">
         <input type="file"  accept="image/*" multiple name="files" @change="handleInput"  />
     </div>
</div>
</template>

<script>
/* eslint-disable */

export default {
  name: 'App',
  data(){
    return{
       
    }
  },
  methods:{
    handleInput(e){
      console.log('onchange event is :', e)
      console.log('files obj is :', e.target.files)
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.input-field{
   background-color: aqua;
   height: 200px;
   display: flex;
   justify-content: center;
   align-items: center;
}
</style>
