# Collection

引入样式时用~开头引入alia里面的缩写地址
路由引入页面 component:resolve => require(['@/views/tradeStatus'], resolve)


````javascript
<style type="text/css">
html,body{width: 100%;height: 100%;}	
*{padding: 0;margin: 0;box-sizing: border-box;}
ul{font-size: 0;}
li{display: inline-block;position: relative;width: 100px;height: 40px;line-height: 40px;font-size: 14px;}
li>a{text-align: center;display: block;}
li:after{content: '';position: absolute;left:100%;width:0;height: 2px;background: #f00;transition: all 0.1s;}
li:hover:after,li.active:after{left: 0;width: 100%;}
li:hover~li:after{left: 0;}
</style>
<ul>
	<li><a href="">1</a></li>
	<li><a href="">2</a></li>
	<li><a href="">3</a></li>
	<li><a href="">4</a></li>
	<li><a href="">5</a></li>
</ul>

````
