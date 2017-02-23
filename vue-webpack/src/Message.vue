<template>
<div> 
  <h1> {{ message }} </h1>
  <app-input :msg="message" @messagechanged="message = $event"></app-input>
  </div>
</template>

<script>
 import Input from './Input.vue';

  export default  {
   data() {
   return {
   message:'my first props'
   }
   },
 	components : {
	 'app-input': Input
 }
 }
</script>