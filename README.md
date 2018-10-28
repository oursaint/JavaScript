<!DOCTYPE html>
<html>
<head>
	<meta charset="utf-8">
	<title></title>
	

</head>

<body onload="startTime()">
	<script type="text/javascript">
		function startTime(){
			var today=new Date()
			var h=today.getHours()
			var m=today.getMinutes()
			var s=today.getSeconds()

			m=checkTime(m)
			s=checkTime(s)
            document.getElementById('txt').innerHTML=h+"点"+m+"分"+s+"秒"
            t=setTimeout('startTime()',500)
         }
         function checkTime(i)
        {
         if (i<10) 
             {i="0" + i}
         return i
         }
	</script>

<div id="txt"></div>

</body>
</html>
