Markdown 是一种轻量级标记语言，它用简洁的语法代替排版，使我们专心于码字。它的目标是实现易读易写，成为一种适用于网络的书写语言。同时，Markdown支持嵌入html标签。

## Markdown 的哲学
John Gruber，知名独立博主，Markdown创始人，UI设计师，苹果狂热粉。</br>

Gruber 认为，Markdown 旨在易读和易写。Markdwon 首先强调可读性。他要求用 Markdown 语法标记后的文本即使不加转换，也能让读者一眼知道哪个是标题，哪段话是重点。所以我们可以看到，Markdown 的语法完全由标点符号组成，标点符号也是经过仔细挑选的。这些符号“看起来就像它们的意思”。例如，我们习惯用星号突出文字内容，在 Markdown 语法里就使用格式*文字*来表示斜体，就算看原文本也能清楚地知道要强调的内容。</br>

另一个强调的则是易写性。这是站在写作者的角度出发的。不管是以何种文体结构题材进行创作，文章的灵感、思路和内容才是最重要的部分。一瞬即逝的灵感要求我们快速记录，并且能较为清晰地把其中逻辑表述出来。这样不至于回头展开内容时忘了顺序，混了情节。

## 基本语法
### 标题
用 # 标记</br>
在标题开头加上1~6个#，依次代表一级标题、二级标题....六级标题。
``` md
#       一级标题
##      二级标题
###     三级标题
####    四级标题
#####   五级标题
######  六级标题
```
</br>

### 强调
两个`*`或着`_`代表加粗，一个`*`或者`-`代表斜体，`~~`代表删除。
``` md
**加粗文本**或者__加粗文本__
*斜体*或者_斜体_
~~删除文本~~
```
效果如下：</br>
~~删除文本~~
</br>

### 代码块
```md
这是行内代码 `onCreate(Bundle savedInstanceState)` 的例子。

这是代码块和语法高亮：

``` java
// 注意java前面有空格
protected void onCreate(Bundle savedInstanceState) {
    super.onCreate(savedInstanceState);
    setContentView(R.layout.activity_main);
}
```
这是行内代码 `onCreate(Bundle savedInstanceState)` 的例子。

这是代码块和语法高亮：

``` java
// 注意java前面有空格
protected void onCreate(Bundle savedInstanceState) {
    super.onCreate(savedInstanceState);
    setContentView(R.layout.activity_main);
}
```
</br>

### 分割线
可以在一行中用三个以上的`*、-、_`来建立一个分隔线，行内不能有其他东西。

```md
***
---
___
```
效果如下
___
</br>

### 换行
使用 html 标签 `</br>` 进行换行。
```md
使用 html 标签`<br/>`<br/>换行
```
</br>

### 图片与链接
图片与链接的语法很像，区别在一个 ! 号。二者格式：
```md
图片：![]()     ![图片文本，可忽略](图片的地址)
链接：[]()      [链接文本](链接地址)    
```