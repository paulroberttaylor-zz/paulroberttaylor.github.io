---
layout: default
comments: true
---

sfdx force:auth:web:login --setdefaultdevhubusername -a DevHub

sfdx force:org:create -f config/project-scratch-def.json -a dap

sfdx force:org:open -u dap

sfdx force:package:install -i 04t6A000000EfcP  -u dap
