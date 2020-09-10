<template>
  <div>
    <navigation/>
    <div class="content">
      <Nuxt />
    </div>
  </div>
 
</template>
<script>
import navigation from '../components/navigation'
export default {
  components:{
    navigation
  }
}
</script>
<style>
*{
  box-sizing: border-box;
  color:whitesmoke;

}
body{
  background: #2d3436;
  color:whitesmoke;
  font-family: Arial, Helvetica, sans-serif;
}
.content{
  padding: 2rem;
}
</style>
