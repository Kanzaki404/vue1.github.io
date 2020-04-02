<template>
  <div class="home">
   
      <div class="content">
        <Snippet />
      </div>
    
  </div>
</template>

<script>
// @ is an alias to /src
import Snippet from '@/components/snippet.vue'

export default {
  name: 'Home',
  components: {
    Snippet
  }
}
</script>


<style scoped>

  .home{
    padding-top: 50px;
  }
  .content{
    background-color: rgba(0, 0, 0, 0.5);
    height: 700px;
    width: 1100px;
    margin-left: 50px;
    margin: auto auto auto 150px;
   color: grey;
    overflow: auto; 
    border-radius: 5px;
  }
</style>