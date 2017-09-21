---
title: Dreamhouse App in a scratch org
layout: post
comments: true
published: true
---

To prepare for creating UI tests using the new Lightning Testing Service, the Dreamhouse app needs to be installed into a scratch org.

Follow the instructions here: [DreamhouseApp SFDX](https://github.com/dreamhouseapp/dreamhouse-sfdx)


Open the new scratch org
``` 
sfdx force:org:open -u dap
```

Select DreamHouse from the app launcher

<img src="{{ site.url }}/assets/gifs/dreamhouse-app-via-sfdx.gif" />


![]({{ site.url }}/assets/gifs/dreamhouse-app-via-sfdx.gif)

Navigate directly to the Proprties list
```
sfdx force:org:open -u dh -p /one/one.app#/sObject/Property__c/list?filterName=Recent
```

