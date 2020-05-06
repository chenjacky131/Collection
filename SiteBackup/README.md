# Collection

websocket服务器 wss://echo.websocket.org/

你给它发什么你都会给你返回什么
3w点看
1. 博百万项目PC端手机端改版（bbw011）
2. 聊天室(bbw011)
  a. 私聊
  b. 多角色
  c. 发送表情,图片
  d. @功能
3. 开奖网(167kjw)
4. 皇冠体育(bbw011)

1. vue项目搭建
2. node项目搭建，mondodb使用；node爬虫
3. python爬虫
4. 个人网站，博客
````javascript
(function(){  
  //  响应式代码
  /*
    sass里面设置转换函数$px为设计图里面的尺寸
    @function p2r($px)
    @return $px/100 + rem
    //  const pixelRatio = window.devicePixelRatio ? window.devicePixelRatio : 1; 设置完initial后好像不需要考虑pixelRatio的值
  */
  window.addEventListener('resize', function(){
    setHtmlFontSize();
  }, false)
  function setHtmlFontSize(){
    const psdWidth = 750 //  设计图尺寸
    const clientWidth = document.documentElement.clientWidth || window.innerWidth;
    document.querySelector('html').style.fontSize = clientWidth / psdWidth * 100 + 'px'// 样式里面的rem单位设置需要除以100是因为chrome字体不能小于6px，为了兼容这个。
  }
  setHtmlFontSize();
}());
````
