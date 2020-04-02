<template>
    <div class="form">
        <h2>Post new Snippet</h2>
        <form id="form1"> 
            <input type="text" id="title" placeholder="Title">
            <textarea name="content" id="content" cols="30" rows="20" placeholder="Content"></textarea>
               
        </form>
         <div class="controls">
                    <button class="btn btn1">Upload</button>
                    <button class="btn btn2">Cancel</button>          
                </div>
    </div>
</template>


<style scoped>

h2{
    color: chartreuse;
}
.form{
    padding: 20px;  
}

input {
    width: 500px;
    padding: 12px 20px;
    margin: 8px 0;
    
    background-color: rgba(0, 0, 0, 0.5);
    border: darkgreen 1px solid;
    color: chartreuse;
}

textarea{  
    background-color: rgba(0, 0, 0, 0.5);
    border: darkgreen 1px solid;
    color: chartreuse;
    padding: 12px 20px;
    width: 500px;
    
}

::placeholder{
    color: chartreuse;
}
.controls{
    float: right;
    padding-top: 10px;   
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
    
}
.btn1 {
        background-color: black ;
        color: #4CAF50; 
        border: 1px solid #4CAF50;
    }

    .btn1:hover {
        background-color: #4CAF50;
        color: white; 

    }

    .btn2 {
        background-color: black; 
        color: red; 
        border: 1px solid red;
    }

    .btn2:hover {
        background-color: red;
        color: white;
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