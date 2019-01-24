# lightbox图片画廊全屏预览插件
# 引入文件
link rel="stylesheet" type="text/css" href="lightbox.css" <br>
<script type="text/javascript" src="jquery.js"></script><br>
<script type="text/javascript" src="lightbox.js"></script><br>
# 在html元素内定义相应的属性开启功能
1.class="js-lightbox"表示这个元素要启用lightbox<br>
2.data-role="lightbox"表示这个元素要启用lightbox<br>
3.data-source="images/2-1.jpg" 原图的地址<br />
4.data-group="group-2"标识当前是否属于一个组别<br />
5.data-id="ghfh"图片的唯一标识<br />
6.data-caption="nghnhg"当前图片的描述文字<br />
# 在单个元素上启用(保持这个元素的data-group和data-id唯一)
<img<br>
class="js-lightbox"<br>
data-role="lightbox"<br>
data-source="images/1-1.jpg"<br>
src="images/1-1.jpg"<br>
data-group="group-1"<br>
data-id="kwhdiuqwdhiu"<br>
data-caption="这么美的风景，是否让你窒息！"<br>
width="100"<br>
height="100"<br>
/><br>
# 给一组元素应用画廊(保持data-group相同)
一组图片<br>
<img<br>
class="js-lightbox"<br>
data-role="lightbox"<br>
data-group="group-2"<br>
data-caption="俄方未婚夫而更为富人前无古人后突然威风威风"<br>
data-id="sdfsdfw"<br>
data-source="images/2-1.jpg"<br>
src="images/2-1.jpg"<br>
width="100px"<br>
height="100px"<br>
/>
<img<br>
class="js-lightbox"<br>
data-role="lightbox"<br>
data-group="group-2"<br>
data-caption="俄方未婚夫但如果热过头热狗热管威风威风"<br>
data-id="fgdgre"<br>
data-source="images/2-2.jpg"<br>
src="images/2-2.jpg"<br>
width="100px"<br>
height="100px"<br>
/><br>
# 创建图片画廊
<script><br>
  $(function() {<br>
    var lightbox = new LightBox({<br>
      speed: 300,<br>
      maxWidth: 900,<br>
      maxHeight: 600,<br>
      maskOpacity: 0.04<br>
    });<br>
  });<br>
</script><br>
