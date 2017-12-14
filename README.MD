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
  <div style="width:500px;">div (Ôø×æ¸¸ÔªËØ)
    <ul>ul (×æ¸¸ÔªËØ)  
      <li>li (¸¸ÔªËØ)
        <span>span</span>
      </li>
    </ul>   
  </div>

  <div style="width:500px;">div (×æ¸¸ÔªËØ)   
    <p>p (¸¸ÔªËØ)
        <span>span</span>
      </p> 
  </div>
</div>

</body>
</html>