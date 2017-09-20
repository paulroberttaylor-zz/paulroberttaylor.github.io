---
title: Creating a scratch org
layout: post
comments: true
published: true
---

_Assuming that a dev org has already been authorised using **sfdx force:auth:web:login**_

Create a new project
``` 
sfdx force:project:create -n YOUR_PROJECT_NAME
```

Enter the newly created directory
```
cd YOUR_PROJECT_NAME
```

Create a new scratch org
``` 
sfdx force:org:create -f config/project-scratch-def.json -a YOUR_SCRATCH_ORG_ALIAS
```

View the list of orgs
```
sfdx force:org:list
```