---
layout: post
title: Javascript Objects
date: May 23, 2014
category: code
comments: true
customid: week8technicalblog
---

####Object Literals 

#####Syntax

```
{							
  "property 1": value1,	
  property2: value2,		
  number: value3			
}							
```
#####Example

```
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
```
#####Property Access 

```
Syntax
name1[string]
name2.identifier
```
#####Example

```
obj['name'];  // 'Hing'
obj.name;     // 'Hing'
obj.getAge(); // 25
```