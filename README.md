# resume
<html>
<head>
<title>hello</title>
<style>/* Stylesheet 1: */
body {
    font: 100% Lucida Sans, Verdana;
    margin: 20px;
    line-height: 50px;
}

.container {
    xmin-width: 900px;
}

.wrapper {
    position:absolute;
    overflow: auto;
}

#top, #sidebar, #bottom, .menuitem {
    border-radius: 4px;
    margin: 4px;
}

#top {
    background-color:green;
    color: #ffffff;
    padding: 15px;
}

#menubar {
    width: 200px;
    float: left
}

#main {
    padding: 10px;
    margin: 0 210px;
}

#sidebar {
    background-color: green;
    color: #ffffff;
    padding: 10px;
    width: 180px;
    bottom: 0;
    top: 0;
    right: 0;
    position: absolute;
}

#bottom {
    border: 1px solid #d4d4d4;
    background-color:green;
    text-align: center;
    padding: 10px;
    font-size: 70%;
    line-height: 14px;
}

#top h1, #top p, #menulist {
    margin: 0;
    padding: 0;
}

.menuitem {
    background-color:white;
    border: 1px solid #d4d4d4;
    list-style-type: none;
    padding: 2px;
    cursor: pointer;
}

.menuitem:hover {
    background-color: #ffffff;
}

.menuitem:first-child {
   background-color:#4CAF50;
   color: white;
   font-weight:bold;
}

a {
    color: #000000;
    text-decoration: underline;
}

a:hover {
    text-decoration: none;
}


@media (max-width: 800px) {
    #sidebar {
        width: auto;
        position: relative;
    } 
     #main {
        margin-right: 0;
    }    

       
}

@media (max-width: 600px) {
    #menubar {
        width: auto;
        float: none;
    }
     #main {
        margin: 0;
    }  
   
}
</style>


</head>

<body>
<div class="container wrapper">
  <div id="top">
    <h1>MY RESUME</h1>
    <p>Use the menu to select </p>
  </div>
  <div class="wrapper">
   <div id="menubar">
     <ul id="menulist">
       <li class="menuitem" onclick="reStyle(0)">Education
       <li class="menuitem" onclick="reStyle(1)">College and School
       <li class="menuitem" onclick="reStyle(2)">Additional skills
       <li class="menuitem" onclick="reStyle(3)">Personal details
       <li class="menuitem" onclick="noStyles()">Invalid
     </ul>
    </div>
</div>
</div>


<h3 align="center">Name:Akshatha P</h3>
<img src="1559534360566.jpg"alt="akshatha's profile picture" height="250" weight="250">
<p></p>


<p><em>I am a student </em>studying in Siddaganga Institute of Technology.</p>
<p>I am a developer with both frontend and backend knowledge</p>

<h4>Phone no:</h4><p>7760536951</p>
 
    
   
 
<hr>
<h2>Education</h2>
<p><li>10th cbse marks obtained is 10 cgpa</li></p>
<p><li>2nd puc marks obtained is 95.2 percent</li></p>
<hr>
<h2>College and School</h2>
<p>I studied in Sri chaitanya techno school and done my intermediate at Sarvodaya college and</p>
<p> later I studied in Siddaganga institute of technology(CSE)</p>
<hr>

<h2>Personal details</h2>

<h4>email<a href="mailto:akshatha.prakash9@gmail.com">email link</a></h4>
<h4>facebook<a href="www.facebook.com\Akshatha Prakash">facebook profile</a></h4>
<hr>
<h2>Additional skills</h2>

<li>Microsoft Office Suite</li>
<li>Accuracy and attention to detail</li>
<li>Time management</li>
<hr>
<a href="my further details">my further details</a>
<hr>
<script>
function noStyles() {
    document.styleSheets[0].disabled = true;
    document.styleSheets[1].disabled = true;
    document.styleSheets[2].disabled = true;
    document.styleSheets[3].disabled = true;
}

function reStyle(n) {
    noStyles()
    document.styleSheets[n].disabled = false;
}

function closeBlackdiv() {
    var blackdiv, stylediv;
    blackdiv = document.getElementById("blackdiv")
    blackdiv.parentNode.removeChild(blackdiv);
    stylediv = document.getElementById("stylediv")
    stylediv.parentNode.removeChild(stylediv);
}

function showStyle(n) {
var div, text, blackdiv;
blackdiv = document.createElement("DIV");
blackdiv.setAttribute("style","background-color:#000000;position:absolute;width:100%;height:100%;top:0;opacity:0.5;margin-left:-20px;");
blackdiv.setAttribute("id","blackdiv");
blackdiv.setAttribute("onclick","closeBlackdiv()");
document.body.appendChild(blackdiv);
div = document.createElement("DIV");
div.setAttribute("id","stylediv");
div.setAttribute("style","background-color:#ffffff;padding-left:5px;position:absolute;width:auto;height:auto;top:100px;bottom:50px;left:200px;right:200px;overflow:auto;font-family: monospace; white-space: pre;line-height:16px;");
text = document.createTextNode(document.getElementsByTagName("STYLE")[n].innerHTML);
div.appendChild(text);
document.body.appendChild(div);
//alert(document.getElementsByTagName("STYLE")[n].innerHTML);
}
reStyle(0);
</script>

</body>
</html>
