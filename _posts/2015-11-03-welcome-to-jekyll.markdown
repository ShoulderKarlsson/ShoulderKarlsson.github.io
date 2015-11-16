---
layout: post
title:  "Blog #1: Precompiling CSS"
date:   2015-11-03 13:13:03
categories: jekyll update
comments: true
---

#What do you think of precompiling your CSS?
Because I've never worked with anything like this before I think this is a really interesting model of CSS.
Since the precompiling offers you to use both variables and functions inside your code I feel
like the workflow might get abit smoother and might even go faster. Although, if you are
unfamiliar with all the SASS functionality and how it works, it might slow you down. But I feel
that if you learn everything correctly I dont see myself using regular CSS if SASS is a valid option
for the project at that time.


* ####Compare to regular CSS
If you compare it to regular CSS there is some big additions. For example, SASS gives you the option to use
something called "mixins". If you know JavaScript you can compare a "mixins" to a function. Another really interesting
feature that is presented is variables. This makes changes more effective and fast. Why this is so effective is
because you only have to change the specific value at just one place. There is another feature that I think needs to be mentioned, nested CSS code.
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
But now I'm more familiar with the concept.

* ####Pros and Cons?
* ####Pros
One of the big Pros with SASS is efficiency. For example, you are way more free to divide your SASS code into separate files.
Of course, this is also an option with regular CSS. But, if you have a bunch of CSS files that results in more link tags wich increases loading time.
This is where SASS really shines and the "compile" situation is being a team player! What I'm talking about is that when you compile your
different files, SASS compiles it into one gigantic CSS file. You might wonder why this is so special, since you can write all your original CSS in one gigantic file.
Sure, there is nothing wrong with that. But since CSS files have a tendency to be very long very fast, a big file can get pretty frustrating to work with.
Me, personally always split my CSS into separate files.
* ####Cons
One of the big perks of CSS (and HTML) is the simplicity. The only thing you need is a text-IDE, a browser and you are ready to go! However
if you choose SASS you need to setup everything which in my opinion removes the simplicity of HTML and CSS and gives it a "Take of Distance".


#What do you think of static site generators?
In general, I really like the concept. One part that I grew fond of was that in the very beginning of your project there already was something on your screen and not just a blank white page.
Which as my personal opinion is really pleasant. Sometimes, I think that it can queit exhausting that you always have to start from a blank white page.

#What is robots.txt and how have you configured it for your site?
robots.txt is a sort of guard for your website. The web is full of "Web Wanderers".
What these wanderers does is that they scan your website and its content, for example search engines use them.
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
usually twitter or github. Since I'm the only one that has been working on this blog, mine humans.txt is quiet short.

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

#What is Open Graph and how did you make us if it?
Open graph is a very clever way when it comes to advertising your website in the context
of social media flows. You use with a couple of meta tags and it creates a perfect "object" when you share your website.
The way to implement Open Graph protocol is through a couple meta tags. These meta tags allow you to integrate your website into the Graph of social media such as facebook.
