---
title: Markdown 语法
date: 2015-10-01 23:32:04
tags: "Markdown"
---

### 1. 斜体和粗体

使用 \* 和 \*\* 表示斜体和粗体。
示例：
这是 *斜体*，这是 **粗体**。

### 2. 分级标题

使用 === 表示一级标题，使用 — 表示二级标题。
示例：
```
这是一个一级标题
============================
这是一个二级标题
--------------------------------------------------
### 这是一个三级标题
```
 你也可以选择在行首加井号表示不同级别的标题 (H1-H6)，例如：`# H1, ## H2, ### H3，#### H4。`

### 3. 外链接

使用 \[描述\]\(链接地址\) 为文字增加外链接。
示例：
这是去往 [本人博客](http://blog.qinchao.me) 的链接。

### 4. 无序列表

使用 *，+，- 表示无序列表。
示例：
 - 无序列表项 一
 - 无序列表项 二
 - 无序列表项 三

### 5. 有序列表

使用数字和点表示有序列表。
示例：
 1. 有序列表项 一
 2. 有序列表项 二
 3. 有序列表项 三

### 6. 文字引用

使用 \> 表示文字引用。
示例：
> 野火烧不尽，春风吹又生。

### 7. 行内代码块

使用 \`代码\` 表示行内代码块。
示例：
让我们聊聊 `html`。

### 8. 代码块

使用 四个缩进空格 表示代码块。
示例：

				这是一个代码块，此行左侧有四个不可见的空格。

有行号的\`\`\`代码块\`\`\`
```shell
$ sudo apt-get install vim-gnome
```

Python 示例：

```python
@requires_authorization
def somefunc(param1='', param2=0):
    '''A docstring'''
    if param1 > param2: # interesting
        print 'Greater'
    return (param2 - param1 + 1) or None

class SomeClass:
    pass

>>> message = '''interpreter
... prompt'''
```

JavaScript 示例：

```javascript
/**
* nth element in the fibonacci series.
* @param n >= 0
* @return the nth element, >= 0.
*/
function fib(n) {
  var a = 1, b = 1;
  var tmp;
  while (--n >= 0) {
    tmp = a;
    a += b;
    b = tmp;
  }
  return a;
}

document.write(fib(10));
```





### 9. 插入图像

使用 \!\[描述\]\(图片链接地址\) 插入图像。
示例：
![百度logo](https://www.baidu.com/img/bd_logo1.png)

### 10. 删除线

使用 ~~ 表示删除线。
~~这是一段错误的文本。~~


### 11. 表格支持
表格内容
```
| 项目        | 价格   |  数量  |
| --------   | -----:  | :----:  |
| 计算机     | \$1600 |   5     |
| 手机        |   \$12   |   12   |
| 管线        |    \$1    |  234  |
```
显示为

| 项目        | 价格   |  数量  |
| --------    | -----: | :----: |
| 计算机      | \$1600 |   5    |
| 手机        |   \$12 |   12   |
| 管线        |    \$1 |  234   |


### 12. Html 标签

Markdown 语法中嵌套 Html 标签，譬如，你可以用 Html 写一个纵跨两行的表格：
html内容
```html
<table>
    <tr>
        <th rowspan="2">值班人员</th>
        <th>星期一</th>
        <th>星期二</th>
        <th>星期三</th>
    </tr>
    <tr>
        <td>李强</td>
        <td>张明</td>
        <td>王平</td>
    </tr>
</table>
```
显示为
<table>
    <tr>
        <th rowspan="2">值班人员</th>
        <th>星期一</th>
        <th>星期二</th>
        <th>星期三</th>
    </tr>
    <tr>
        <td>李强</td>
        <td>张明</td>
        <td>王平</td>
    </tr>
</table>
