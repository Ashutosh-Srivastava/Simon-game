# Simon-game

## What is jQyery?
`$("h1")` is equivalent to `jQuery("h1")` it is just to reduce the number of lines of code that you are typing.

## Incorporate jQuery in websites
- Use the CDN(Content Delivery Network) of google from jQuery website.

- If you are placing the script tag in the head section place the jQuery script above the javaScript script tag and use the following way 
to build the .js file:
```
$(document).ready(function() {
  $("h1").css("color","red");
}); 
```
- **The best way is to use the CDN is place it at the end inside the body tag.**

## Minified version
Minified version ignores all the comments and spaces from the code to reduce the size of file.
[Minifier](www.minifier.org) can be used to produce your minified version of code. The extension is **.min**

The $("some tag") is equivalent to DOM's `querySelector()` and `querySelectorAll()`.
To change the css styles we use `$("#head h1").css("font-size","3rem");`
Here the css property name will be same as that in css irrespective of what used in DOM.
`$("#head h1").css("font-size")` this would give the font-size.

`$("h1").addClass("big margin")` add multiple class witch space in between:
- `removeClass()` to remove class
- `hasClass()` to check for particular class

`$("h1").text()` and `$("h1").html()` to manipulate text content and html respectively.

`$("a").attr("href","random site address")` to change the attributes.

`$("a").attr("class")` to print the classes attached.

## Using Event Listeners
`$("h1").click(<callback function>)` to add event listeners.

Another way of adding event listener is `$("h1").on("event-listener",callback function)`.

## Adding html 
`$("h1").<method>(<add HTML>)` where methods can be before, after, append and prepend.

## Animations in jQuery
Some common animations are:
- fadeOut
- fadeIn
- fadeToggle
- slideUp
- slideDown
- slideToggle
- hide
- show
- toggle
usage: `$("button").click(function(){});`

### Another way is using animate to style our css
```
$("button").on("click", function(){
	$("h1").animate({opactity: 0.5});
});
```
i.e on clicking the button the text in H1 tag gets a CSS property defined.

- we can also add multiple animations to a tag eg.
```
$("button").on("click", function(){
	$("h1").slideUp().slideDown().animate({opactity: 0.5});
});
```

## More effects
For jQuery effect methods refer to this link [w3schools](https://www.w3schools.com/jquery/jquery_ref_effects.asp) or [jQuery official](https://api.jquery.com/category/effects/)
