---
layout: post
title:  "第一篇Jekyll博客"
date:   2016-11-16 23:09:48 +0800
categories: jekyll update
---
You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

{% highlight ruby %}
def show
@widget = Widget(params[:id])
  respond_to do |format|
    format.html # show.html.erb
    format.json { render json: @widget }
  end
end
{% endhighlight %}
引用图片和资源
[截图一]({{site.url}}/assets/canvas.png )
pdf文件下载 ：你可以直接下载[xiazai pdf]({{site.url}}/assets/abc2.pdf)

<img src="{{siteurl}}/assets/canvas.png"/>
