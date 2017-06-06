<!DOCTYPE html>

<html lang = "zh-TW">

<head>

	<title>專題</title>
	<meta charset = "utf-8">
	
	<style>
		
		body
		{
			background: black;
		}
		
		img
		{
			width: 15%;
			height: 15%;
		}
		
		canvas
		{
			background: white;
			padding: 0;
			margin: auto;
			display: block;
			position: absolute;
			top: 0;
			bottom: 0;
			left: 0;
			right: 0;
			
		}
		
	</style>
	
	<script type="text/javascript">

		window.onload = function() {
			var canvas = document.getElementById("myCanvas");
			var ctx = canvas.getContext("2d"); 
			var img = new Image();   	
			img.onload = function(){
				ctx.drawImage(img, 0, 0);
			};	
			img.src = 'source/sky.png'; // Set source path
			
			var dialog = new Image();   	
			dialog.onload = function(){
				ctx.drawImage(dialog, 520, 650);
			};	
			dialog.src = 'source/dialog3.png'; // Set source path
		}
		
	</script>

</head>

<body>
	
	<img src = "source/title.png">
	
	</img>
	<canvas id="myCanvas" width="1280" height="720">
	
	</canvas>
	
</body>

</html>

