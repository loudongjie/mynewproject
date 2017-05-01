# mynewproject
<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<title>随机数、时间控制</title>
		<script>

	// 11.27作业第二题实现随机选取10–100之间的10个数字，存入一个数组并在页面中显示输出实现随机选取10–100之间的10个数字，存入一个数组并在页面中显示输出
	// window.onload=function(){
	// 	var arr=new Array(10);
	// 	for (var i = 0; i < 10; i++) {
	// 		arr[i]=Math.floor(Math.random(0,1)*90+10);
	// 	};
	// 	document.write(arr);
	// }


	//11.27 作业第三题在文本框中显示当前时间，可以停止，也可以继续。请写出实现此功能的代码（html代码和js代码）
	var a=function(){
		var time1=document.getElementById('time');
		var time2=new Date();
		time1.value=time2.getHours()+":"+time2.getMinutes()+":"+time2.getSeconds(); 
	}
	var b;
	b=setInterval(a,1000);
	var sstart=function(){
		b=setInterval(a,1000);
	}
	var sstop=function(){
		clearInterval(b);
	}
	</script>
</head>
<body>
	<input type="text" id="time">
	<input type="button" onclick="sstart()" value="开始" style="background-color:lightblue">
	<input type="button" onclick="sstop()" value="停止">
</body>
</html>
