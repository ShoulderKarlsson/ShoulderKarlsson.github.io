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

* ####Which techniquies did you use?
When I designed my blog the only thing I took advantage of was variables.
Alot of things where already implemented in Jekyll as standard. Since I found the concept
of mixins and calculations inside CSS very interesting I wrote some of my own, I didn't end up using any of them.
But I'm not more familiar with the concept.

* ####Pros and Cons?
* ####Pros
One of the big Pros with SASS is efficiency. For example, you are way more free to divide your SASS code into separate files.
Of course, you are as free as you want to be in regular CSS. But, if you a bunch of CSS files that results in more link tags.
This is where SASS really shines and the "compile" situation is being a team player! What I'm talking about is that when you compile your
different files, SASS compiles it into one gigantic CSS file. You might wonder why this is so special, since you can write all your original CSS in one gigantic file.
Sure, there is nothting wrong with that. But since CSS files have a tendency to be very long very fast, a big file can get pretty frustrating to work with.
Me, personally always split my CSS into separate files.
* ####Cons
One of the big perks of CSS (and HTML) is the simplicity. The only thing you need is a text-IDE, a browser and you are ready to go!
This was almost the only con that I could come to think of. Since SASS needs to be compiled, you cant just open your IDE and write something. The "Take off distance".


#What do you think of static site generators?
In general, I really like the concept. One part that I grew fond of fast was that you see result on the screen the second you load the website.
Which as my personal opinion is really pleasant. Sometimes, I think that it can queit exhausting that you always have to start from a blank white page.

#What is robots.txt and how have you configured it for your site?
robots.txt is a sort of guard for your website. The web is full of "Web Wanderers".
What these wanderers does is that they scan your website and its content. Search engines uses these for example.
If you don't want your website to show when you are searching for example on Bing. You can use it to disallow the robots
Bing uses for their search on content. Roughly can say that robots.txt works like a bouncer at a nightclub. It decides who's allowed in or not allowed.

* #####Below you can see my robots.txt
{% highlight bash %}
User-agent: *
Disallow: /
{% endhighlight %}

#What is humans.txt and how have you configured if for your site
In general, humans.txt is just a fun feature that you can implement for your website. What it does is that you can mention the people that
has been working on your website, for example. You can mention their names, what their task was on the site and how you can contact them,
usually twitter, github. Since I'm the only one that has been working on this blog, mine humans.txt is quiet short.

* #####Below you can see the humans.txt I've used.
{% highlight bash %}

/* TEAM */

Webmaster: Axel Karlsson
mail: ak223fy@student.lnu.se
github: ShoulderKarlsson

/* SITE */
Last update: 2015-11-11
Language: English
Doctype: HTML5
IDE: Atom, Jekyll, Liquid and SCSS

{% endhighlight %}

#How did you implement comments to the blog?
We used a service called 'disqus'. The process to implement was really straight forward
and not that complicated. The first thing you had to do was create a account on disqus so you can handle the comment section.
After your account was ready you got a piece of JavaScript code that you could paste at the location you wanted able to comment.
This is where Jekyll really shines. Since the blog posts follow the same layout, the obvious place to implement the code was in the layout for posts.

#What is open graph and how did you make us if it?
