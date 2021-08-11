HTML

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="styles.css">
    <link rel="stylesheet" href="path/to/font-awesome/css/font-awesome.min.css">

</head>
<body>
   <nav>
   
<div class="container">
    <h2>background color:<span id="color">#f1f5f8</span></h2>
    </div>
    <div class="bt">
    <input type="button" id="btn" value="click me">

</div>
<script src="index.js"></script>
</body>


CSS:

.center{
    display:flex;
    text-align: center;
    justify-content: center;
    align-items: center;
    flex-direction: column;

}

.center ul li{
    display:inline-block;
    padding:7px;
    text-decoration: none;
    margin: 23px;

}

.center ul li a{
    color:black;
    text-decoration-line: none;
    text-shadow: 2em;
}


.container{
    border:2px solid black;
    display: inline-block;
    text-align: center;
    justify-content: center;
    align-items: center;
    margin-left: 523px;
background-color: black;
color:rgb(87, 87, 158);
margin-top: 177px;
padding: 8px 34px;
}

#btn{
margin-left: 662px;
margin-top:20px;
border-radius:2px;
background-color:black;
color:white;
padding:10px 10px;

}

#btn:hover{
    background-color: rgb(4, 19, 42);
    color:rgb(42, 146, 149);
    cursor: pointer;
}

JAVASCRIPT
const colors=['#F6A9A9','#BD4B4B',"#BD4B4B","#E93B81"];//defined different colors
const btn=document.getElementById('btn');//variable for button
const color=document.getElementById('color');// to show the color change as well on the display

btn.addEventListener('click', function(){// when clicked
    //call the funtion//


  
  document.body.style.backgroundColor=colors[randomColor()];// add differnt colors from the variable colors on top

    color.innerHTML=colors[randomColor()]// also change the words to which color we are usign

   
})
function randomColor(){// function
    return Math.floor(Math.random()*colors.length);// show random colors 
}

