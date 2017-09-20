---
title: Dreamhouse App in a scratch org
layout: post
comments: true
published: true
---

To prepare for creating UI tests using the new Lightning Testing Service, the Dreamhouse app needs to be installed into a scratch org.

_Assuming that a dev org has already been authorised using **sfdx force:auth:web:login**_

1. ```bash sfdx force:project:create -n DreamhouseAppTesting```
2. sfdx force:org:create -f config/project-scratch-def.json -a dap
3. sfdx force:package:install -i 04t6A000000EfcP  -u dap
4. sfdx force:org:open -u dap


<img src="{{ site.url }}/assets/gifs/dreamhouse-app-via-sfdx.gif" />


