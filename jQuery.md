jQuery
jQuery is a fast and concise JavaScript library created by John Resig in 2006. jQuery simplifies HTML document traversing, event handling, animating, and Ajax interactions for Rapid Web Development.
Affects html elements, html events handling for the elements.
JS is purely Object oriented language and all in js are objects ie methods and members.
```
Installation
<script type = "text/javascript" src = "/jquery/jquery-2.1.3.min.js">
or
<script type = "text/javascript" 
         src = "https://ajax.googleapis.com/ajax/libs/jquery/2.1.3/jquery.min.js">
```
Basics
Call the jQuery
Initialize the ready event for the document
```
$(document).ready(function() {
   // do stuff when DOM is ready
});
Context
$(document).ready(function() {
   // this refers to window.document
});
$("div").click(function() {
   // this refers to a div DOM element
});
```

Selectors
```
$("p").css("background-color", "yellow");
$("#id").css("background-color", "yellow");
$(".class").css("background-color", "yellow");
```
Attribute
```
$(document).ready(function() {
            $("#myimg").attr("src", "/jquery/images/jquery.jpg");
  $("em").addClass("selected");
var content = $(this).html();
         });
 ```
Attribute methods – attr, removeattr, hasclass, removeclass, html, text, val, etc
Traverse the li elements
```
$("li").eq(2).addClass("selected");
$("p").find("span").addClass("selected");
```
Events
```
$('div').bind('click', function( event ){
               alert('Hi there!');
            });
 ```
//for unbinding
```
selector.unbind(eventType, handler)
Event methods – preventdefault – prevents browser from executing default action
```
Also can use, on, click, blur etc for the event binding
Ajax
```
[selector].load( URL, [data], [callback] );
$('#stage').load('/jquery/result.html', {"name":name}
);
[selector].getJSON( URL, [data], [callback] );
$.getJSON('/jquery/result.json', function(jd) {
                  $('#stage').html('<p> Name: ' + jd.name + '</p>');
```
Other methods: ajax, get, post, serializes,etc 
Events: ajaxstart, ajaxcomplete,etc
Effects 
```
[selector].show( speed, [callback] );
$(".target").toggle('slow', function(){
```
jQuery - theming
