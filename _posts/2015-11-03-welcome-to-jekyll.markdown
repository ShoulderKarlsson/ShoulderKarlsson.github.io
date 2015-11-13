---
layout: post
title:  "Blog #1"
date:   2015-11-03 13:13:03
categories: jekyll update
comments: true
---

#What do you think of precompiling your CSS?
Think I've never worked with anything like this before I think this is a really interesting model of CSS.
Since the precompiling bit offers you to use both variables and functions inside your code I feel
like the workflow might get abit smoother and might even go faster. When you are pretty new to the
SASS workflow with Mixins and such other it might slow you down, but when you get use to it I don't se
myself go back to regular CSS.

* ####Compare to regular CSS
If you compare it to regular CSS there is some big additions. For example, SASS gives you the option to use
something called "mixins". If you know JavaScript you can compare a "mixins" to a function. Another really interesting
feature that is presented is variables. This makes changes more effective and fast. Because you only need to change
the specific value in just one place. There is another feature that I think needs to be mentioned, nested CSS code.
For me, this was amazing. When I first saw an example I thought it was so much easier to read and much easier to grasp.
* #####Below I'll show you an example of nested CSS code

{% highlight CSS %}
#foo {
  height:100px;
  width:100px;
  background-color: #e4e4e4;
  
  #bar {
    height:inherit;
    width:50px;
    background-color: #33bada;
  }
}
{% endhighlight %}
