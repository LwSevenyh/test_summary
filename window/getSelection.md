## Window.getSelection
>返回一个 Selection 对象，表示用户选择的文本范围或光标的当前位置。

### 语法
```
const selection = window.getSelection()
```

> *String.toString()* 方法 
获取鼠标被选中的文本，返回字符串

### 示例
```
function foo() {
    let selObj = window.getSelection(); 
    let selText = selObj.toString();
    console.log(selText);
}
```

>Document.getSelection()，两个方法等价
目前在Firefox, Internet Explorer 中，getSelection() 对 **textarea** 及 **input** 元素不起作用。 
HTMLInputElement.setSelectionRange() 或 selectionStart 及 selectionEnd 属性可用于解决此问题。
