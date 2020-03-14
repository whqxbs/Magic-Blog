用到的工具：

1、Aplayer
其实很简单，Github有很多大神开源了相关的内容。用着最舒服的，当属Aplayer了，可以去官网体验一下：

https://aplayer.js.org/

文档手册也很翔实：

https://github.com/MoePlayer/APlayer

方法很简单，加载Aplayer的js和css，在想要展先的位置调用即可。Aplayer支持很多模式，上图展示的效果为吸底模式，就是在网页的页面最左下角展示。我以吸底模式为例进行说明，如果想采用其它模式，可以根据文档手册修改代码。

2、Meting
如果只使用Aplayer，那么需要指定音乐的图片地址，mp4地址，歌词等，用着不是很方便，这时就可以使用Meting作为辅助：

https://github.com/metowolf/MetingJS

Meting为Aplayer提供了网易云音乐的API接口，只要获得网易云音乐歌单的ID，就可以自动加载歌单里所有的歌曲，直接调用，方便很多，当然除了网易云音乐的API，还有其他的接口。

使用方法：

APlayer.min.css、APlayer.min.js、Meting.min.js放到你知道的地方（雾

在主题的footer.php中加入如下代码

```
<link rel="stylesheet" href="path-to/css/APlayer.min.css">
<script src="path-to/js/APlayer.min.js"></script>
<div class="aplayer"
    data-id="2507749822"
    data-fixed="true"
    data-server="netease"
    data-volume="0.4"
    data-type="playlist">
</div>
<script src="path-to/js/Meting.min.js"></script>
```

path-to记得替换成自己的路径

data-id是网易云的歌单

效果可以去我的博客看一看