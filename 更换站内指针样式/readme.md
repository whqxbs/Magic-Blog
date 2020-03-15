十分简单的更换方式，这里用默认指针和超链接指针举例子

在 WordPress后台-外观-自定义-额外CSS 中加入以下CSS：


/** 普通指针样式**/
body {
cursor: url(http://xxx/mouse1.png), default;
}
 
/** 链接指针样式**/
a:hover{cursor:url(http://xxx/mouse2.png), pointer;
}

xxx换成鼠标图片的url

这里有我正在用的初音未来的两个，效果见我的博客.