<template>
    <div>
        <ul>
            <li><a href="#">Latest</a></li> |
            <li><a href="#">Most Upvoted</a></li> 
        </ul> 
        <div class="container">      
            <h2>Title</h2>
            <div class="content">
                <p>Lorem ipsum dom ipsum dolor sit amet consectetur adipisicing elit. Commodi natus quia reiciendis, cupiditate aliqm ipsum dolor sit amet consectetur adipisicing elit. Commodi natus quia reiciendis, cupiditate aliqm ipsum dolor sit amet consectetur adipisicing elit. Commodi natus quia reiciendis, cupiditate aliqm ipsum dolor sit amet consectetur adipisicing elit. Commodi natus quia reiciendis, cupiditate aliqm ipsum dolor sit amet consectetur adipisicing elit. Commodi natus quia reiciendis, cupiditate aliqm ipsum dolor sit amet consectetur adipisicing elit. Commodi natus quia reiciendis, cupiditate aliqm ipsum dolor sit amet consectetur adipisicing elit. Commodi natus quia reiciendis, cupiditate aliqm ipsum dolor sit amet consectetur adipisicing elit. Commodi natus quia reiciendis, cupiditate aliqm ipsum dolor sit amet consectetur adipisicing elit. Commodi natus quia reiciendis, cupiditate aliqm ipsum dolor sit amet consectetur adipisicing elit. Commodi natus quia reiciendis, cupiditate aliqm ipsum dolor sit amet consectetur adipisicing elit. Commodi natus quia reiciendis, cupiditate aliqm ipsum dolor sit amet consectetur adipisicing elit. Commodi natus quia reiciendis, cupiditate aliqm ipsum dolor sit amet consectetur adipisicing elit. Commodi natus quia reiciendis, cupiditate aliqm ipsum dolor sit amet consectetur adipisicing elit. Commodi natus quia reiciendis, cupiditate aliqm ipsum dolor sit amet consectetur adipisicing elit. Commodi natus quia reiciendis, cupiditate aliqm ipsum dolor sit amet consectetur adipisicing elit. Commodi natus quia reiciendis, cupiditate aliqm ipsum dolor sit amet consectetur adipisicing elit. Commodi natus quia reiciendis, cupiditate aliqm ipsum dolor sit amet consectetur adipisicing elit. Commodi natus quia reiciendis, cupiditate aliqm ipsum dolor sit amet consectetur adipisicing elit. Commodi natus quia reiciendis, cupiditate aliqm ipsum dolor sit amet consectetur adipisicing elit. Commodi natus quia reiciendis, cupiditate aliqm ipsum dolor sit amet consectetur adipisicing elit. Commodi natus quia reiciendis, cupiditate aliqm ipsum dolor sit amet consectetur adipisicing elit. Commodi natus quia reiciendis, cupiditate aliqm ipsum dolor sit amet consectetur adipisicing elit. Commodi natus quia reiciendis, cupiditate aliqm ipsum dolor sit amet consectetur adipisicing elit. Commodi natus quia reiciendis, cupiditate aliqm ipsum dolor sit amet consectetur adipisicing elit. Commodi natus quia reiciendis, cupiditate aliqm ipsum dolor sit amet consectetur adipisicing elit. Commodi natus quia reiciendis, cupiditate aliqlor sit amet consectetur adipisicing elit. Commodi natus quia reiciendis, cupiditate aliquid quam minus? Numquam animi consequuntur ad beatae quasi consequatur, quisquam distinctio eos! Architecto temporibus dignissimos omnis?</p>
            </div>
            <button class="btn btn1">Vote Up</button>
            <button class="btn btn2">Vote Down</button>          
            <button class="btn btn2 btnR">Delete</button>
            <div class="rating">
                <p id="upvotes">+ 2</p>
                <p id="downvotes">- 3</p>
            </div>        
        </div>  
    </div>
</template>

<script>
export default {
    name: 'Snippet'
}
</script>

<style scoped>

    .rating{
        display: flex;
    }
    #upvotes{
        color: chartreuse;
    }
    #downvotes{
        color: red;
        
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