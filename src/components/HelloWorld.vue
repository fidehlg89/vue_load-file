<template>
  <div>
    <span>Test Image</span>
    <img :src="image" alt="">
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  
  data(){
    return {
        image: require("../assets/logo.png") 
    }
  },
  methods:{
    imageChange(e){
      console.log(e);
    }
  }
}
</script>
