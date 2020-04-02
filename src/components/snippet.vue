<template>
    <div>
       
            <ul>
                <li><a href="#" @click="getLatest">Latest</a></li> |
                <li><a href="#" @click="getMostUpvoted">Most Upvoted</a></li> 
            </ul> 
            <div class="container" v-for="snippet in snippets" v-bind:key="snippet.id" >      
                <h2>{{snippet.title}}</h2>
                <div class="content">
                    <p>{{snippet.content}}</p>
                </div>
                <button class="btn btn1" @click="voteUp(snippet.id)">Vote Up</button>
                <button class="btn btn2" @click="voteDown(snippet.id)">Vote Down</button>          
                <button class="btn btn2 btnR" @click="del(snippet.id)">Delete</button>
                <div class="rating">
                    <p id="Score">Score : {{snippet.score}}</p>
                    <p id="id">ID: {{snippet.id}}</p>
            </div>        
        </div>
    </div>

</template>

<script>
import axios from 'axios'
const url = 'https://www.forverkliga.se/JavaScript/api/api-snippets.php?';
export default {
    
    name: 'Snippet',
    data(){
        return {
            snippets: []
        }
    },
    methods: {
        getLatest(){
            axios.get('https://www.forverkliga.se/JavaScript/api/api-snippets.php?latest')
            .then(res => this.snippets = res.data)
            .catch(err => console.log(err))
           
        },
        getMostUpvoted(){
            axios.get('https://www.forverkliga.se/JavaScript/api/api-snippets.php?best')
            .then(res => this.snippets = res.data)
            .catch(err => console.log(err))
            console.log(this.snippets)
        },
        voteUp(id){ //something is wrong
            console.log('vote up called with id:' + id)
            axios.post(url, { upvote:'', id:id})
            .then(res => console.log(res.data.message))
            .catch(err => console.log(err))
          
        },
        voteDown(id){
            console.log('vote down called with id:  ' + id)
            axios.post(url,{downvote:'', id:id })
            .then(res => console.log(res.data.message))
            .catch(err => console.log(err))           
        },
        del(id){
            console.log('delete called with id:  ' + id )
            axios.post(url, {delete:'',id:id})
            .then(res => console.log(res.data.message))
            .catch(err => console.log(err))
            
        }

    },
    created(){
            axios.get('https://www.forverkliga.se/JavaScript/api/api-snippets.php?latest')
            .then(res => this.snippets = res.data)
            .catch(err => console.log(err))
            console.log(this.snippets)
    }   

}
</script>

<style scoped>

    .rating{
        display: flex;
    }
    #Score{
        color: chartreuse;
    }
    #id{
        color: chartreuse;
        
    }
    ul{
        list-style-type: none;
        float: right;
        padding:0px 10px 30px 5px;
        color: green;
    }

    li{
        display: inline;
    }
    a{
        color: chartreuse;
        text-decoration: none;
    }

    a:hover{
        text-decoration: underline;
    }

    h2{
        float: left;
        padding: 10px;
        color: chartreuse;
    }
    .container{
        width: 900px;
        min-height:200px;
        height: auto;
        margin: 50px auto 150px auto;
    }

    .content{
        background-color: #2a3439;
        min-height:200px;
        height: 300px;
        width: 870px;
        margin: 50px auto 10px 10px;
        overflow: auto; 
        border: 1px solid chartreuse;
        color: rgb(192, 192, 192);
        
    }

    .btn {
        background-color: #4CAF50; /* Green */
        border: none;
        color: white;
        padding: 7px 32px;
        text-align: center;
        text-decoration: none;
        /* display: inline-block; */
        font-size: 16px;
        margin: 7px 7px;
        transition-duration: 0.4s;
        cursor: pointer;
        float: left;
    }
    .btn1 {
        background-color: #151a1c ;
        color: #4CAF50; 
        border: 1px solid #4CAF50;
    }

    .btn1:hover {
        background-color: #4CAF50;
        color: white; 

    }

    .btn2 {
        background-color: #151a1c; 
        color: red; 
        border: 1px solid red;
    }

    .btn2:hover {
        background-color: red;
        color: white;
    }

    .btnR{
        float: right;
        margin-right:18px;
    }


    p{
        padding: 15px;
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