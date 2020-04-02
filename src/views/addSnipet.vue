<template>
  <div class="add">
    
    <div class="content">
      <newSnippet/>
    </div>
  </div>
</template>
<script>
import newSnippet from '@/components/newSnippet.vue'
export default {
    components:{
      newSnippet
    } 
}
</script>

<style scoped>
  .add{
    padding-top: 50px;
    
  }
  .content{
    
    height: 600px;
    text-align: center;
    width: 600px;
    margin-left: 50px;
    margin: auto ; 
    overflow: auto; 
    border-radius: 5px;
  }

  
</style>