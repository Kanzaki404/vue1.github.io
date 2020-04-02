<template>
    <div>
        <ul>
            <li><a href="#">Latest</a></li> |
            <li><a href="#">Most Upvoted</a></li> 
        </ul> 
        <div class="container">      
            <h2>Title</h2>
            <div class="content">
                <p>Lorem ipsum dolor sit amet r sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicinr sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet cr sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officietur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officig elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officiconsectetur adipisicing elit. Eos provident vitae harum possimus officia perferendis quas dolorem hic ut praesentium itaque impedit aspernatur asperiores molestias animi odio, eligendi quod ipsam?</p>
            </div>
            <button class="btn btn1">Vote Up</button>
            <button class="btn btn2">Vote Down</button>          
            <button class="btn btn2 btnR">Delete</button>
            <div class="rating">
                <p id="upvotes">+ 2</p>
                <p id="downvotes">- 3</p>
            </div>        
        </div>


        <div class="container">      
            <h2>Title</h2>
            <div class="content">
                <p>Lorem ipsum dolor sit amet r sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicinr sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet cr sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officietur adipisicing elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officig elit. Eos provident vitae harum possimus officir sit amet consectetur adipisicing elit. Eos provident vitae harum possimus officiconsectetur adipisicing elit. Eos provident vitae harum possimus officia perferendis quas dolorem hic ut praesentium itaque impedit aspernatur asperiores molestias animi odio, eligendi quod ipsam?</p>
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
        min-height:300px;
        height: auto;
        
        margin: 50px auto 150px auto;
    }

    .content{
        background-color: rgba(0, 0, 0, 0.6);
        min-height:200px;
        height: 300px;
        width: 870px;
        margin: 50px auto 10px 10px;
        overflow: auto; 
        border: 1px solid chartreuse;
        
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
        background-color: transparent ;
        color: #4CAF50; 
        border: 2px solid #4CAF50;
    }

    .btn1:hover {
        background-color: #4CAF50;
        color: white; 

    }

    .btn2 {
        background-color: transparent; 
        color: red; 
        border: 2px solid red;
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
</style>