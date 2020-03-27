部署全站pjax的好处是加快访问速度，同时配合音乐控件解决了打开新帖子音乐中断的问题（更多好处请百度）

我采用的是一种比较简单的全站部署方法，不同的主题会出现不一样的小问题，可以自己借助js去调整页面CSS

把pjax.js丢到服务器上，在footer.php中加入以下代码

<script src="路径/pjax.js"></script>

这一条是引入js

<script> 
 $(document).pjax('a[target!=_blank]', '#main-container', {fragment:'#main-container', timeout:8000}); 
</script>

这一条是部署全站标签，#main-container需要自己去首页上利用F12找，一般离<body>很近,可以在我的博客里观察#main-container的位置
