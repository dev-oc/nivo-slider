Nivo Slider is "The Most Awesome jQuery Image Slider". See http://nivo.dev7studios.com for more info.





Nivoslider插件参数和方法一览表
参数/方法  描述	默认值
基本
effect	图片切换效果。提供了11种效果：'sliceDownRight','sliceDownLeft','sliceUpRight','sliceUpLeft', 'sliceUpDown','sliceUpDownLeft', 'fold','fade','slideInRight','slideInLeft'，诸如渐入渐出，滑动，百叶窗等等都有。	random
animSpeed	图片切换速度（毫秒）	500
pauseTime	图片停留时间（毫秒）	3000
startSlide	开始切换的位置（即从第几张图开始切换）。	0
directionNav	是否使用左右按钮导航	true
directionNavHide	是否当鼠标滑上图片时出现左右导航按钮	true
controlNav	是否使用导航控制条，即显示每张图片的按钮	true
controlNavThumbs	是否使用缩略图控制导航	false
controlNavThumbsFromRel	是否使用图片的rel属性关联缩略图	false
controlNavThumbsSearch	缩略图类型	'.jpg'
controlNavThumbsReplace	缩略图后缀	'_thumb.jpg'
keyboardNav	是否支持键盘方向键切换（貌视IE不支持）	true
pauseOnHover	当鼠标滑向图片时，停止切换	true
manualAdvance	是否不自动切换，当为true时，需要手动切换	false
captionOpacity	设置图片标题说明的背景透明度	0.8
方法
beforeChange	当发生切换前，回调函数	 
afterChange	当发生切换后，回调函数	 
slideshowEnd	完成所有的切换动作后，回调函数	 
lastSlide	切换最后一张图片时，回调函数	 
afterLoad	当加载完成时，回调函数






 <script type="text/javascript" src="jquery.nivo.slider.pack.js"></script>
    <script type="text/javascript">
    $(window).load(function() {
        $('#slider').nivoSlider({
                effect:'random', //图片切换效果。提供了11种效果：'sliceDownRight','sliceDownLeft','sliceUpRight','sliceUpLeft', 'sliceUpDown','sliceUpDownLeft', 'fold','fade','slideInRight','slideInLeft'，诸如渐入渐出，滑动，百叶窗等等都有。
  			animSpeed:300,
				pauseTime:1500,
				directionNav:true,//是否使用导航控制条，
				controlNavThumbs:true,//是否使用缩略图控制导航
				controlNavThumbsFromRel:true,
				pauseOnHover:true,//当鼠标滑向图片时，停止切换
				manualAdvance:false,//	是否不自动切换，当为true时，需要手动切换
				captionOpacity:0.7,//	设置图片标题说明的背景透明度	0.8
				//beforeChange	当发生切换前，回调函数	 
				//afterChange	当发生切换后，回调函数	 
				//slideshowEnd	完成所有的切换动作后，回调函数	 
				//lastSlide	切换最后一张图片时，回调函数	 
				//afterLoad	当加载完成时，回调函数				
		});		 
    });
    </script>
