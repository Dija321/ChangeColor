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

