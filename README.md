# webpage
#This is my  personal webpage using HTML5, CSS and JS. 
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
<script>
 $(document).ready(function() {
 $("button").click(function() {
 $(".bottom").animate({right:'0%'},2000);
 $(".bottom").queue(function() {
 $(".bottom").css("background-color","yellow");
 $(".bottom").dequeue();
 })
 $(".bottom").animate({left:'0%'},2000);
 $(".bottom").queue(function() {
 $(".bottom").css("background-color","green");
 $(".bottom").dequeue();
 })
 $(".bottom").animate({bottom:'0%'},2000);
 $(".bottom").queue(function() {
 $(".bottom").css("background-color","blue");
 $(".bottom").dequeue();
 })
 $(".bottom").animate({top:'0%'},2000)
 $(".bottom").queue(function() {
 $(".bottom").css("display","none");
 $(".bottom").dequeue();
 })
 });
 });
</script>
<title>Document</title>
<style>
 .top {
 height: 100px;
 }
 .parent {
 position: relative;
 height: 600px;
 }
 .bottom {
 height: 150px;
 width: 150px;
 text-align: center;
 background-color: red;
 position: absolute;
 /* display: flex;
 justify-content: center;
 align-items: center; */
 }
 .hello {
 font-size: 20px;
 }
 button {
 margin-bottom: 30px;
 }
</style>
</head>
<body>
<div class="top">
 <h1>19BIT0130 PIYUSH KUMAR</h1>
</div>
<button>CLICK ME</button>
<div class="parent">
 <div class="bottom">
 <div class="hello">
 Hello VITian
 </div>
 </div>
</div>
</body>
</html>
