project_path: /web/_project.yaml
book_path: /web/fundamentals/_book.yaml
description: 响应式网页设计模式正在快速发展，但只有少数几种成熟的 模式可以在桌面和 和移动设备上流畅运行

{# wf_review_required #}
{# wf_updated_on: 2014-10-20 #}
{# wf_published_on: 2000-01-01 #}

# Mostly fluid {: .page-title }

{% include "_shared/contributors/TODO.html" %}



Mostly fluid 模式主要由流动网格组成。  在较大和中等屏幕上 ，它通常保持相同大小，只在更宽的 屏幕上调整边距。

在较小屏幕上，流动网格使主内容重排，
同时各列垂直排列。  此模式的一个主要优点是，
在小屏幕和大屏幕之间通常只需要一个
视图断点。

{% link_sample _code/mostly-fluid.html %}
  <img src="imgs/mostly-fluid.svg">
  试一下
{% endlink_sample %}

在最小的视图中，每个内容 `div` 都垂直排列。  在屏幕
宽度达到 600px 时，主要内容 `div` 保持 `width: 100%`，而辅助
`div` 在主要 `div` 下面显示为两列。  宽度超过
800px 时，窗口 `div` 变为固定宽度并在屏幕上居中。

使用此模式的网站包括：

 * [A List Apart](http://mediaqueri.es/ala/)
 * [Media Queries](http://mediaqueri.es/)
 * [SimpleBits](http://simplebits.com/)


<pre class="prettyprint">
{% includecode content_path="web..//fundamentals/design-and-ui/responsive/patterns/_code/mostly-fluid.html" region_tag="mfluid" lang=css %}
</pre>

