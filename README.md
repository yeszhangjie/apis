# APIs 笔记



API是什么
- API是英文Application Program Interface的缩写。翻译：应用程序接口
- 应用程序接口：接口就是一种方法、一种途径。
- API是一种统称的叫法。

JS的组成部分：
- ECMAScript: 语法  制定者：ECMA 欧洲计算机协会
- DOM：Document Object Model 文档对象模型。制定者：W3C
- BOM：Browser Object Model 浏览器对象模型。


# DOM

## DOM是什么
- Document Object Model 文档对象模型。制定者：W3C
- 创建时间：文档对象模型是在当前文档加载之后创建的。
- 文档对象模型把文档一切内容描述为对象(树状对象)。
    - 根对象：Document对象。是DOM的根对象。
    - 元素对象：Element对象。 把文档种的所有标签描述成元素对象。
    - 文本对象：Text对象。把文档中全部字符(可见|不可见)描述为文本对象。
    - 属性对象：Attribute对象。把文档种的全部标签的属性描述为属性对象。
    - DOM还为浏览器的内置事件添加了处理程序。
- DOM的用途：用于操作HTML文档。（操作：增、删、改、查）

DOM树状结构示意图
![DOM树](blob/main/images/ct_htmltree.gif)


## Document对象

**定义**
- Document对象表示整个web文档。
- Document对象是页面种其他所有对象的主人。
- Document对象DOM的根对象，也是访问页面内容的入口。

**Dcoument对象属性**
document.documentElement
document.head
document.title
document.body

**Dcoument对象方法**
- document.getElementById()
- document.getElementsByClassName()
- document.getElementsByTagName()
- document.querySelector()
- document.querySelectorAll()

- document.createElement(element) 创建 HTML 元素
- element.removeChild(element)	删除 HTML 元素
- element.appendChild(new) //添加HTML元素（从后添加）
- element.insertBefore(new,old) //添加HTML元素（从前添加）

**重要的话**

一旦从文档中选取了一个元素之后，很多时候需要基于此元素查找与之相关的元素，此时DOM提供了两种API可供使用：
- 节点对象树
- 元素对象树

## Node对象树
- 节点就是Node，Node就是节点。
- 文档中的一切内容都是节点。
    - 根对象节点：document对象
    - 元素对象： 文档中的每一个HTML元素
    - 属性对象：每一个标签的属性
    - 文本对象： 每一个标签的内容
    - 注释对象： 注释
- 子节点：在一个节点之下的直接节点（属性对象例外）
- 父节点：在一个节点之上的直接节点。

**Node对象属性**
- Node.childNodes :查询子节点
- Node.parentNode :查询父节点
- Node.firstChild :查询第一个子节点
- Node.lastChild :查询最后一个子节点
- Node.nextSibling :查询下一个兄弟节点
- Node.previousSibling :查询上一个兄弟节点
- Node.nodeType : 查询节点类型
    - 1: #element
    - 2: #attribute
    - 3: #text
    - 8: #comment
    - 9: #document
- Node.nodeName: 查询节点的名称
- Node.nodeValue: 查询节点的值


**Node对象方法**


## Element对象



**Element对象属性**
- Element.children :返回所有子元素对象（忽略其他类型的节点对象）
- Element.parentElement :查询父元素
- Element.firstElementChild :查询第一个子元素
- Element.lastElementChild :查询最后一个子元素
- Element.nextElementSibling :查询下一个兄弟元素
- Element.previousElementSibling :查询上一个兄弟元素

**Element对象方法**
- Element.querySelector()
- Element.querySelectorAll()



# BOM


