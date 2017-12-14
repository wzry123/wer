<!DOCTYPE html>
<html>
<head>
<meta charset="utf-8">
<style>
.ancestors *
{ 
	display: block;
	border: 2px solid lightgrey;
	color: lightgrey;
	padding: 5px;
	margin: 15px;
}
</style>
<script src="http://cdn.static.runoob.com/libs/jquery/1.10.2/jquery.min.js">
</script>
<script>
$(document).ready(function(){
  $("span").parent().css({"color":"red","border":"2px solid red"});
});
</script>
</head>
<body>

<div class="ancestors">
  <div style="width:500px;">div (曾祖父元素)
    <ul>ul (祖父元素)  
      <li>li (父元素)
        <span>span</span>
      </li>
    </ul>   
  </div>

  <div style="width:500px;">div (祖父元素)   
    <p>p (父元素)
        <span>span</span>
      </p> 
  </div>
</div>

</body>
</html>
<!DOCTYPE html>
<html>
<head>
<meta charset="utf-8">
<style>
.descendants *
{ 
	display: block;
	border: 2px solid lightgrey;
	color: lightgrey;
	padding: 5px;
	margin: 15px;
}
</style>
<script src="http://cdn.static.runoob.com/libs/jquery/1.10.2/jquery.min.js">
</script>
<script>
$(document).ready(function(){
  $("div").children("p.1").css({"color":"red","border":"2px solid red"});
});
</script>
</head>
<body>

<div class="descendants" style="width:500px;">div (当前元素) 
  <p class="1">p (儿子元素)
    <span>span (孙子元素)</span>     
  </p>
  <p class="2">p (儿子元素)
    <span>span (孙子元素)</span>
  </p> 
</div>

</body>
</html>
<html>
<head>
<meta charset="utf-8">
<script src="http://cdn.static.runoob.com/libs/jquery/1.10.2/jquery.min.js">
</script>
<script>
$(document).ready(function(){
	$("div p").last().css("background-color","yellow");
});
</script>
</head>
<body>

<h1>欢迎访问我的主页</h1>
<div>
	<p>这是 div 中的一个段落。</p>
</div>

<div>
	<p>这是另外一个 div 中的一个段落。</p>
</div>

<p>这是一个段落。</p>

</body>
</html>