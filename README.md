# dirSlide
可以跟踪鼠标移动方向的滑动插件
###说明
1.应用对象ul,id必须是dirList  
2.此版本是beta版本，可能存在Bug;  
3.**仅用于交流和学习，不作商业用途。**  
4.与我联系：[淡忘~浅思](http://www.ido321.com)   [久艾分享](http://blog.92fenxiang.com)  欢迎交流  
5.相关文章：[JS判断鼠标进入容器的方向](http://blog.92fenxiang.com/articles/1427022777)  

###使用说明
#####如何使用
依赖于JQuery，所以要先引入JQuery，一个简单示例：

```javascript
<!DOCTYPE HTML>
<html lang="en-US">
<head>
<meta charset="UTF-8">
<title>dirSlide</title>

<script src='http://libs.baidu.com/jquery/1.9.0/jquery.js'></script>
</head>
<body>

    <ul id='dirList'>
        <li><img src='1.jpg'/><div>图片一</div></li>
        <li><img src='2.jpg'/><div>图片二</div></li>
        <li><img src='3.jpg'/><div>图片三</div></li>
        <li><img src='4.jpg'/><div>图片四</div></li>
        <li><img src='5.jpg'/><div>图片五</div></li>
    </ul>
      <h3 style="text-align:center">交流：<a href="http://www.ido321.com" target="_blank">dwqs</a></h3>

<script type="text/javascript" src="./dirSlide.min.js"></script>
<script>
    $("#dirList").dirSlide();
</script>
</body>
</html>
```
效果请戳：[Demo](http://test92.sinaapp.com/dirSlide/dirslide.html)

#####一些参数
可以给dirSlide()传入一个对象参数，参数列表如下：
<table>
    <thead>
        <tr>
            <td>参数</td>
            <td>说明</td>
            <td>默认值</td>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>wrapbg</td>
            <td>设置#dirList的背景色</td>
            <td>null</td>
        </tr>
        <tr>
            <td>lisdis</td>
            <td>设置#dirList的子元素li之间的margin，设置时不需要带单位</td>
            <td>10</td>
        </tr>
        <tr>
            <td>width</td>
            <td>li元素的宽度，设置时不需要带单位</td>
            <td>null</td>
        </tr>
        <tr>
            <td>height</td>
            <td>li元素的高度,设置时不需要带单位</td>
            <td>null</td>
        </tr>
        <tr>
            <td>fontname</td>
            <td>遮罩的字体名</td>
            <td>Microsoft Yahei</td>
        </tr>
        <tr>
            <td>opacity</td>
            <td>遮罩的透明度</td>
            <td>0.7</td>
        </tr>
        <tr>
            <td>lisbg</td>
            <td>遮罩的背景色</td>
            <td>#0C0E0C</td>
        </tr>
        <tr>
            <td>fontsize</td>
            <td>遮罩的字体大小，设置时不需要带单位</td>
            <td>25</td>
        </tr>
        <tr>
            <td>color</td>
            <td>遮罩的字体颜色</td>
            <td>#FFF</td>
        </tr>
        <tr>
            <td>anitime</td>
            <td>遮罩动画变化时间</td>
            <td>200</td>
        </tr>
        <tr>
            <td>outtime</td>
            <td>setTimeout的间隔时间</td>
            <td>200</td>
        </tr>
    </tbody>
</table>

修改默认的参数
```javascript
<!DOCTYPE HTML>
<html lang="en-US">
<head>
<meta charset="UTF-8">
<title>dirSlide2</title>

<script src='http://libs.baidu.com/jquery/1.9.0/jquery.js'></script>
</head>
<body>

    <ul id='dirList'>
        <li><img src='1.jpg'/><div>图片一</div></li>
        <li><img src='2.jpg'/><div>图片二</div></li>
        <li><img src='3.jpg'/><div>图片三</div></li>
        <li><img src='4.jpg'/><div>图片四</div></li>
        <li><img src='5.jpg'/><div>图片五</div></li>
    </ul>
      <h3 style="text-align:center">交流：<a href="http://www.ido321.com" target="_blank">dwqs</a></h3>

<script type="text/javascript" src="./dirSlide.min.js"></script>
<script>
    $("#dirList").dirSlide({
    	lisbg:"#AD087C",
        color:"#000",
        anitime:"1000",
        opacity:"0.5",
        wrapbg:"#CCC"
    });
</script>
</body>
</html>
```
演示地址：<http://test92.sinaapp.com/dirSlide/dirSlide2.html>
