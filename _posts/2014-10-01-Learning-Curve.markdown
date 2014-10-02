---
layout: post
title:  "Learning Curve"
date:   2014-10-01 22:14:20
categories: jekyll update
---

We entered our second day of JavaScript today, and I feel like my brain is starting to stretch.

The assignment for today was much different than those we've been working with over the past week. Thus far, we've been given visual cues and asked to recreate them with markup and styling. This kind of thing really falls within my comfort zone, coming from a design background and being a visual learner. However, today we were given a data set.

This thing was just one massive array, 'items'. Here's a link to the [monstrosity](https://github.com/tiy-atlanta-js/Assignments/blob/master/Assignment%2006/items.js). When Tim first showed us the code, it took a full 20 seconds to scroll all the way through the file. Lots and lots of data.

Our job was to access this array with JavaScript and have our consoles log a number of it's specific qualities to the console. One problem required that we access the properties within an array  of materials that was stored within each object within the array of items. This one gave me fits, but seems so simple once you see it:

{% highlight javascript %}
// Log items that are made of wood

items.forEach(function(a){
    a.materials.forEach(function(b){
        if(b === "wood"){
            console.log(a.title);
        };
    });
});
{% endhighlight %}

Shout out to [Max](http://maxehnert.github.io/) for helping me wrap my simple brain around this one.

I feel like we are getting into the real programming at this point. It's very exciting, but a little daunting. Doesn't feel like drowning quite yet, but definitely getting my feet wet.