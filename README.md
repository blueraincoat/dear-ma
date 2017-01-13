<!doctype html>
<html lang="zh">
<head>
	<meta charset="UTF-8">
	<meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1"> 
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<title>CSS animation-play-state属性效果演示|DEMO_jQuery之家-自由分享jQuery、html5、css3的插件库</title>
	<link rel="stylesheet" type="text/css" href="css/normalize.css" />
	<link rel="stylesheet" type="text/css" href="css/htmleaf-demo.css">
	<style type="text/css">
		.clock {
		  align-items: center;
		  border-radius: 50%;
		  border: solid 15px DarkTurquoise;
		  display: flex;
		  height: 200px;
		  justify-content: center;
		  margin: 80px auto 0;
		  width: 200px;
		  margin: 80px auto 0;
		}

		.hand {
		  align-items: center;
		  background: DarkTurquoise;
		  border-radius: 50%;
		  display: flex;
		  height: 20px;
		  justify-content: center;
		  width: 20px;
		  z-index: 2;
		}

		.clock:hover .hand:after {
		  animation-play-state: paused;
		  -webkit-animation-play-state: paused;
		  cursor: pointer;
		}

		.hand:after {
		  content: '';
		  height: 80px;
		  width: 8px;
		  background: DarkTurquoise;
		  border-radius: 4px;
		  top: -40px;
		  position: relative;
		  -webkit-animation: timer 4s linear infinite;
		  animation: timer 4s linear infinite;
		  transform-origin: 48% 100%;
		  -webkit-transform-origin: 48% 100%;
		  animation-play-state: paused;
		  -webkit-animation-play-state: running;
		}

		@-webkit-keyframes timer {
		  0% {
		    -webkit-transform: none;
		    transform: none;
		  }
		  100% {
		    -webkit-transform: rotate(360deg);
		    transform: rotate(360deg);
		  }
		}
		@keyframes timer {
		  0% {
		    -webkit-transform: none;
		    transform: none;
		  }
		  100% {
		    -webkit-transform: rotate(360deg);
		    transform: rotate(360deg);
		  }
		}

	</style>
	<!--[if IE]>
		<script src="http://libs.useso.com/js/html5shiv/3.7/html5shiv.min.js"></script>
	<![endif]-->
</head>
<body>
	<div class="htmleaf-container">
		<header class="htmleaf-header">
			<h1>CSS animation-play-state属性效果演示</h1>
			<div class="htmleaf-links">
				<a class="htmleaf-icon icon-htmleaf-home-outline" href="http://www.htmleaf.com/" title="jQuery之家" target="_blank"><span> jQuery之家</span></a>
				<a class="htmleaf-icon icon-htmleaf-arrow-forward-outline" href="http://www.htmleaf.com/ziliaoku/qianduanjiaocheng/201603233254.html" title="返回下载页" target="_blank"><span> 返回下载页</span></a>
			</div>
		</header>
		<div class='clock'>
		  <div class='hand'></div>
		</div>
	</div>
</body>
</html>
