##360度3D汽车旋转

####1.引入js文件

	<script src="js/jquery.min.js"></script>
	<script src="js/circlr.js"></script>
####2.书写样式

	<div class="container">
		<div id="circlr">
			
		</div>
	</div>
####3.书写JavaScript代码

	<script>
	for (var i = 1; i <= 70; i++) {
		// var cir = document.getElementById('circlr');
		//创建Img
		var img = document.createElement('img');
		//添加到页面中
		$('#circlr')[0].appendChild(img);
		//设置值
		img.setAttribute('data-src', 'picture/'+i+'.png');
	}
	
	$(function(){
		var cir = circlr('circlr',{
			scorll:true,
		});
	});	
	</script>

这样就可以实现汽车旋转了。
图片文件以及源代码：[https://github.com/Goorln/car-rotate.git](https://github.com/Goorln/car-rotate.git)
