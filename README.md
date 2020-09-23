<div align="center">

## Fading Dynamic Content


</div>

### Description

This JavaScript creates a slide-show effect displaying different contents dynamically. The content fades in while being displayed.
 
### More Info
 
This JavaScript creates a slide-show effect displaying different contents dynamically. The content fades in while being displayed.

The script is extremely customisable. You can add any number of messages. You can also change the delay between different messages.

To use the script just copy the <SCRIPT> section of the source of the page and paste it wherever you need it on your web page.


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Premshree Pillai](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/premshree-pillai.md)
**Level**          |Intermediate
**User Rating**    |4.0 (8 globes from 2 users)
**Compatibility**  |
**Category**       |[Layers](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/layers__2-78.md)
**World**          |[Java](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/java.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/premshree-pillai-fading-dynamic-content__2-2843/archive/master.zip)





### Source Code

```
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.0 Transitional//EN">
<html>
<head>
<title>Fading Dynamic Content</title>
<style type="text/css">
.link{font-family:verdana,arial,helvetica; font-size:8pt; color:#003399; font-weight:normal}
.link:hover{font-family:verdana,arial,helvetica; font-size:8pt; color:#0099FF; font-weight:normal}
.header{font-family:arial,verdana,helvetica; font-size:20pt; color:#3366CC; font-weight:bold}
</style>
</head>
<body bgcolor="#FFFFFF">
<center><span class="header">Fading Dynamic Content</span>
<br><br>
<center>
<!--BEGIN FADING DYNAMIC CONTENT SCRIPT-->
<script language="javascript">
// Use Freely as long as following messages are intact ::
//---------------------------------------------------------------
// Fading Dynamic Content JavaScript              |
// This script written and © 2002 Premshree Pillai.       |
// All rights reserved.                     |
// Created on : 28/04/02                    |
// Web : http://www.qiksearch.com/               |
// Mail : premshree@hotmail.com                 |
// FREE JavaScripts at http://www.qiksearch.com/javascripts.htm |
//---------------------------------------------------------------
// Location of script : http://www.qiksearch.com/javascripts/fading-dynamic-content.htm
//--------------------------------------CUTOMISE----------------------------------------------
var qiksearch_js_text = new Array ("Fading Dynamic Content", "by Premshree Pillai", "You can even add<br>multiple lines", "www.qiksearch.com");
var qiksearch_space_width = 390; // The width of the content space
var qiksearch_space_height = 50; // The height of the content space
var qiksearch_space_borderw=3; // Border width
var qiksearch_space_borderc="#CC0000"; // Border Color
var timeOutVal=150; // Delay in milliseconds
//--------------------------------------------------------------------------------------------
//-----------------------------DO-NOT-MODIFY-BELOW-THIS---------------------------------------
document.write('<table width="' + qiksearch_space_width + '" height="' + qiksearch_space_height + '" style="background:#FFFFFF; border:' + qiksearch_space_borderw + ' solid ' + qiksearch_space_borderc + '"><tr><td align="middle">');
document.write('<div id="qiksearch_js_space">');
document.write('</div>');
document.write('</td></tr></table>');
var def_10='A',def_11='B',def_12='C',def_13='D',def_14='E',def_15='F';
var colorVal=15;
var div_count=0;
function qiksearch_fade_desat(getColorIntVal)
{
 var returnVal;
 if(getColorIntVal>=10)
 {
 for(var i=0; i<=15; i++)
 {
  if((getColorIntVal==i))
  {
  returnVal = eval('def_' + i);
  }
 }
 }
 else
 {
 returnVal=getColorIntVal;
 }
 return(returnVal);
}
function writeDiv()
{
 document.all.qiksearch_js_space.innerHTML= '<font face="verdana,arial,helvetica" size="-1" color="' + joinColor(qiksearch_fade_desat(colorVal)) + '"><b>' + qiksearch_js_text[div_count] + '</span></b></font>' ;
 if((colorVal>0) && (colorVal!=0))
 {
 colorVal--;
 }
 else
 {
 colorVal=15;
 if(div_count<qiksearch_js_text.length)
 {
  div_count++;
 }
 if(div_count==qiksearch_js_text.length)
 {
  document.all.qiksearch_js_space.innerHTML = '<a href="javascript:resetAll();writeDiv();" style="text-decoration:none" accesskey="l"><font color="#808080" face="verdana,arial,helvetica" size="-1"><b>P<u>l</u>ay Again <font color="#CC0000">&raquo;</font></b></font></a>';
 }
 }
 if(div_count<qiksearch_js_text.length)
 {
 setTimeout("writeDiv()",timeOutVal);
 }
}
function joinColor(getColor)
{
 return (getColor + '0' + getColor + '0' + getColor + '0');
}
function resetAll()
{
 div_count=0;
 colorVal=15;
}
writeDiv();
</script>
<!--END FADING DYNAMIC CONTENT SCRIPT-->
</center>
<br>
<table width="400" align="center"><tr><td>
<font face="verdana,arial,helvetica" size="-1" color="#000000">
This JavaScript creates a slide-show effect displaying different contents dynamically.
The content fades in while being displayed.
<br><br>The script is extremely customisable. You can add any number of messages. You can also change the delay between different messages.
<br><br>To use the script just copy the &lt;SCRIPT&gt; section of the source of the page and paste it wherever you need it on your web page.
<br><br><hr style="width:100%; height:1px; color:#FF9900">
<a href="http://www.qiksearch.com" class="link">&#169; Copyrights 2002 Premshree Pillai. All rights reserved.</a>
</font>
</td></tr></table>
</body>
</html>
```

