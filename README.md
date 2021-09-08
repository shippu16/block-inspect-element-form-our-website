# block-inspect-element-form-our-website
Use of F12 key on the browser:
This can be blocked using javascript key event listener. Use the below script to do accomplish it.

$(document).keydown(function(e){ 
    if(e.which === 123){ 
 
       return false; 
 
    } 
 
}); 

2. Use of Right click

You can block this using javascript or with just your html

<html oncontextmenu="return false"> 
</html> 
or

$(document).bind("contextmenu",function(e) {  
	e.preventDefault(); 
 
}); 

3. Use of other shortcuts involving Ctrl keys

<body oncontextmenu="return false" onkeydown="return false;" onmousedown="return false;"> 
Your body content 
</body> 
