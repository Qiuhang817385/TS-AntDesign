```js
// 这个CSS属性真心不错
      pointer-events: none;
```

```js

给左侧加边框的同时,消除左侧边框添加上去的影响
可以使用透明边框属性,划入上去之后覆盖掉之前的
>.menu-item {
    border-left: $menu-item-active-border-width solid transparent;
    &.is-active, &:hover {
      border-bottom: 0px;
      border-left: $menu-item-active-border-width solid $menu-item-active-color;
    }
  }
```

## Menu升级

1.只能放入MenuItem组件

2.index默认传入,属性改成非必须



测试的时候,通过render创建的元素,都默认会在最后被调用cleanUp方法然后清除掉

但是在代码的最前面并没有清除



## children是一个不透明的数据结构

循环children的方法

![image-20200612221422223](C:/Users/Artificial/AppData/Roaming/Typora/typora-user-images/image-20200612221422223.png)

map+foreach
