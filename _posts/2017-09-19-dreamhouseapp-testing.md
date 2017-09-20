---
title: Setting up Dreamhouse in a scratch org
layout: default
comments: true
---

# Setting up Dreamhouse in a scratch org

sfdx force:org:create -f config/project-scratch-def.json -a dap

sfdx force:package:install -i 04t6A000000EfcP  -u dap

sfdx force:org:open -u dap


<img src="{{ site.url }}/assets/gifs/dreamhouse-app-via-sfdx.gif" />
