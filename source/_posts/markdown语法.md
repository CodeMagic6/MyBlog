---
title: markdown语法
date: 2017-09-17 22:48:48
tags:
---
# Markdown 语法的简要规则

## 标题
标题有两种风格，SetText和Atx

\# 一级标题
\## 二级标题
\### 三级标题
\#### 四级标题
\##### 五级标题
\###### 六级标题

## 引用
行首使用>加上一个空格表示引用一个段落，可嵌套

>引用
>>引用

## 分割线
在一行连续使用三个或以上_或*
___
***

## 代码区域

代码区域内的文字不会被处理，按照原样输出。
每一行前边加入4个空格或者一个tab可以标记一个代码段落：

    int main() {
        reutrn 0;
    }

## 强调

\*斜体\*
\**粗体\**
\_斜体\_
\__粗体\__

*斜体*
**粗体**
_斜体_
__粗体__

## 链接

    文字链接
    Inline:
    [谷歌](https://www.google.com)
    Reference:
    [谷歌][google_url]
    [google_url]:https://www.google.com

    图像链接
    ![](http://www.google.rw/images/srpr/logo4w.png)
    ![][google_url]
    [google_url]:http://www.google.rw/images/srpr/logo4w.png

## 转义字符

\\ 反斜杠
\` 反引号
\* 星号
\_ 下划线
\{\} 大括号
\[\] 中括号
\(\) 小括号
\# 井号
\+ 加号
\- 减号
\. 英文句号
\! 感叹号

## 列表

\* 无序列表
\+ 无序列表
\- 无序列表

* 无序列表
+ 无序列表
- 无序列表

\1.第一项
\2.第二项

1.第一项
2.第二项