<template>
<div>  
  <VueTreeSelect  v-model="selected" :multiple="true" :options="options"  /> 
</div>
  
</template>

<script setup> 
import VueTreeSelect from './components/Treeselect'
import './../styles/style.less';
import {  ref} from "vue";  
  let selected = ref();
 const  options = ref([ {
          id: 'a',
          label: 'a',
          children: [ {
            id: 'aa',
            label: 'aa',
          }, {
            id: 'ab',
            label: 'ab',
          } ],
        }  ]) 

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
</style>
