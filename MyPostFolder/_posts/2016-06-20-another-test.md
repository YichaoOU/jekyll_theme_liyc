---
layout: post
title: 一些常用的markdown语言
header_keywords_abstract : false
one_sentence: 这里，用一句话总结
header_image: Desert.jpg
---

<hr> 


# 这是一级标题 {#a1}

## 这是二级标题


### 这是三级标题

# 这样写Reference：

TCA循环是生物体很重要的一个代谢过程[^1]

这是一个  `红色的高亮`

## 这是一个  大字号的  `红色的高亮

下面是blockquote

> 好好学习，天天向上
>
> 黄河之水天上来，奔流到海不复还

注意，markdown在书写时，加了特效的地方都要单独成行。
比如下面的例子，他们是连续的三行，则其output是：

# 这是一级标题
## 这是二级标题
### 这是三级标题

<kbd>有底色的文字</kbd>


我喜欢<span class="label label-primary">BootStrap</span>


下面是代码高亮：

{% highlight ruby %}
def show
  puts "Outputting a very lo-o-o-o-o-o-o-o-o-o-o-o-o-o-o-o-ong lo-o-o-o-o-o-o-o-o-o-o-o-o-o-o-o-ong line"
  @widget = Widget(params[:id])
  respond_to do |format|
    format.html # show.html.erb
    format.json { render json: @widget }
  end
end
{% endhighlight %}


这样来添加图片：

![anything](/image/Desert.jpg)

这样来添加链接，你知道什么是[光合作用](https://zh.wikipedia.org/wiki/%E5%85%89%E5%90%88%E4%BD%9C%E7%94%A8)么？

*Italic*

**Bold**

***Bold and Italic***

这样写一个list:

- first
- second
- third

这样来写数学公式:

$$ \sum_{a=0}^{a=N} a+1 $$

设置锚定：

[返回顶部](#a1)

<hr>
[^1]:给出你的reference




