---
layout: post
title: Javascript Objects
date: May 23, 2014
category: code
comments: true
customid: week8html
---

####Object Literals 

#####Syntax

{% highlight ruby %}
{							
  "property 1": value1,	
  property2: value2,		
  number: value3			
}							
{% endhighlight %}
#####Example

{% highlight ruby %}
var obj = {								
  name: "Hing",							
  married: false,							
  "mother's name": "Lynn",					
  "year of birth": 1988,						
  getAge: function () {					
    return 2014 - obj["year of birth"];	
  },										
  1: 'one'									
};											
{% endhighlight %}
####Property Access 


#####Syntax

{% highlight ruby %}
name1[string]
name2.identifier
{% endhighlight %}
#####Example

{% highlight ruby %}
obj['name'];  // 'Hing'
obj.name;     // 'Hing'
obj.getAge(); // 25
{% endhighlight %}