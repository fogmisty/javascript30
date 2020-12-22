# JavaScript30 —— 30 天 JS 挑战

> 官网：https://javascript30.com/

> 参考中文教程：https://github.com/soyaine/JavaScript30

## DAY 1 —— JavaScript Drum Kit

### 知识点

1. 键盘事件

addEventListener 事件监听方法：addEventListener 方法可以将事件处理程序附加到指定元素（DOM 对象，window 对象）；removeEventListener 方法删除事件监听器。

语法：

event: 事件类型，如 click、mousedown

function: 事件发生时调用的函数

useCapture: 布尔值，true 为事件捕获（先外后内），false 为事件冒泡（先内后外）

```
element.addEventListener(event, function, useCapture);
```

2. 声音播放

```
element.play(); // 开始
element.pause(); // 暂停
element.currentTime = 0; // 恢复初始播放时间点
```

3. 样式修改

HTML data-\*属性

HTML DOM classList 属性

```
element.classList.add('class');
element.classList.remove('class');
```

transitionend 需要和 transition 搭配使用

```
// element的样式必须有transition否则无效
element.addEventListener('transitionend', function, useCapture);
```
