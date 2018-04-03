# Collection


### 全屏的监听
```` javascript
		// 监听全屏状态变化的事件
		document.addEventListener("fullscreenchange", function(e) {
			if(IsFull()){
				$("html").removeClass("fullscreen");
			}
		});
		document.addEventListener("mozfullscreenchange", function(e) {
			if(IsFull()){
				$("html").removeClass("fullscreen");
			}
		});
		document.addEventListener("webkitfullscreenchange", function(e) {
			if(!IsFull()){
				$("html").removeClass("fullscreen");
			}
		});
		document.addEventListener("msfullscreenchange", function(e) {
			if(IsFull()){
				$("html").removeClass("fullscreen");
			}
		});
		//判断是否全屏
		function IsFull() {
		    var fullscreenElement =
		        document.fullscreenEnabled
		        || document.mozFullscreenElement
		        || document.webkitFullscreenElement;
		    var fullscreenEnabled =
		        document.fullscreenEnabled
		        || document.mozFullscreenEnabled
		        || document.webkitFullscreenEnabled;
		    if (fullscreenElement == null)
		    {
		        return false;
		    } else {
		        return true;
		    }
		}
````

event.target 是触发事件的元素，而 event.currentTarget 是事件绑定的元素。也就是说，大部分情况下，当使用事件代理时，event.target 是子元素，而 event.currentTarget 是父级元素。
