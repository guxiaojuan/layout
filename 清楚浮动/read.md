####清楚浮动主要有以下几种方法

1. 针对父元素
> 1. 给父元素设置高度
 2. 给父元素设置overflow(hidden或者auto)
 3. 给父元素添加display:table
 4. 给父元素添加伪类
```
   .parent::after {display:block; content: ''; clear: both;}
```

2. 再添加一个空的子元素,设置clear:both;height:0;
```html
  <div parent>
    <div class="son1"></div>
    <div class="son2"></div>
    <div class="clear"></div>
  </div>
```

