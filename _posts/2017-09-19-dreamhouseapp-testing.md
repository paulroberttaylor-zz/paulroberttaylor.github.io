---
title: Setting up Dreamhouse in a scratch org
layout: post
comments: true
published: true
---

# Dreamhouse App in a scratch org

To prepare for creating UI tests using the new Lightning Testing Service, the Dreamhouse app needs to be installed into a scratch org.

_Assuming that a dev org has already been authorised using **sfdx force:auth:web:login**_

- sfdx force:project:create -n DreamhouseAppTesting

- sfdx force:org:create -f config/project-scratch-def.json -a dap

- sfdx force:package:install -i 04t6A000000EfcP  -u dap

- sfdx force:org:open -u dap


<img src="{{ site.url }}/assets/gifs/dreamhouse-app-via-sfdx.gif" />
