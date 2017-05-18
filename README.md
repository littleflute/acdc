 [v0.0.6](https://github.com/littleflute/acdc/edit/master/README.md)
 
[Highway To Hell (REMST)](Highway To Hell [REMST])

<audio controls id="player"> 
  <source src="https://littleflute.github.io/acdc/Highway%20To%20Hell%20%5BREMST%5D/01 Highway To Hell.mp3" type="audio/mpeg">
Your browser does not support the audio element.
</audio>
<div id="xd"> 
</div>
<script>
var d = document.getElementById("xd"); 
var html = d.innerHTML; 
html += " acdc<br>Highway To Hell [REMST]<br>CD:<br>";
for(var n=1; n<=19; n++)
{	
 	html += fNewBtn(n);

} 
d.innerHTML = html;

var p = document.getElementById("player");
function f(i)
{
    var s = "https://littleflute.github.io/acdc/Highway%20To%20Hell%20%5BREMST%5D/";
    if(i==1)
    {
    	s += "01 Highway To Hell";
    }
    else if(i==2)
    {
    	s += "02 Girls Got Rhythm";
    }
    else if(i==3)
    {
    	s += "03 Walk All Over You";
    }
    else if(i==4)
    {
    	s += "04 Touch Too Much";
    }
    else
    {
    	if(i<10) 
    	{
    		s += "0";
    	} 
    	s += i;
    	s += "_曲目 ";
    	s += i;
    }
    s += ".mp3";
    
    p.src = s; 
    p.play();
}
function fNewBtn(i)
{
	var rHTML = "";
    rHTML = "<button onclick='f(";
    rHTML += i;
    rHTML += ");'>";
    rHTML += i;
    rHTML += "</button>";
    return rHTML;
}
</script>


