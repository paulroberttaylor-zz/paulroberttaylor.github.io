---
title: Dreamhouse App in a scratch org
layout: post
comments: true
published: true
---

To prepare for creating UI tests using the new Lightning Testing Service, the Dreamhouse app needs to be installed into a scratch org.


Create a new project which will be used for the Dreamhouse work
``` 
sfdx force:project:create -n DreamhouseAppTesting
```

Enter the newly created directory
```
cd DreamhouseAppTesting
```

Create a new scratch org called dap
``` 
sfdx force:org:create -f config/project-scratch-def.json -a dap
```

Install the Dreamhouse package from [Dreamhouse App](http://www.dreamhouseapp.io/installation/) installation

``` 
sfdx force:package:install -i 04t6A000000EfcP  -u dap
```

Open the new scratch org
``` 
sfdx force:org:open -u dap
```

Select DreamHouse from the app launcher

<img src="{{ site.url }}/assets/gifs/dreamhouse-app-via-sfdx.gif" />


