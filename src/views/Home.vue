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
    /* background-color: rgba(0, 0, 0, 0.5); */
    height: 700px;
    width: 1100px;
    margin-left: 50px;
    margin: auto;
    color: grey;
    overflow: auto; 
    border-radius: 5px;
  }

  ::-webkit-scrollbar {
  width: 5px;
}

/* Track */
::-webkit-scrollbar-track {
  background: rgb(102, 102, 102); 
}
 
/* Handle */
::-webkit-scrollbar-thumb {
  /* background: #888;  */
  background: chartreuse;
}


</style>