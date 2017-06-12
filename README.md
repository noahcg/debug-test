# Debug Test

This repo is being used to work through the debug-test. Below is a list of edits I made to correct the index.html file.

## Edits

Added curly braces around the fancybox object properties. Also added fitToView and autoSize properties to help get the correct modal size to display.

```
$.fancybox({
	href : "#lb_container",
	fitToView : false,
	autoSize : false
});
```
Changed the milliseconds to account for 7 seconds

```
setTimeout( function(){
}, 7000);
```
Removed the double quotes around the expires property value

```
$.cookie('has_viewed_modal', 'yes', { expires: 1 });
```
Added the following CSS to the pre-existing styles for #lb_container

```
#lb_container {
	background: #fff; 
	border-radius: 5px; 
	height: 200px;
	padding: 20px;
}
```
Added/Modified the following CSS to the pre-existing styles for #lb_container a.btn

```
#lb_container a.btn {
	display: inline-block;
	margin-bottom: 20px;
	position: absolute;
}
```