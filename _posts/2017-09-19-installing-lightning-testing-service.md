---
title: Installing Lightning Testing Service
layout: post
comments: true
published: true
---

If the Dreamhouse app has not yet been installed into a scratch org, see [Dreamhouse App in a scratch org]({% post_url 2017/09/19/dreamhouseapp-testing %})

sfdx force:package:install -i 04tJ0000000EbBy  -u dap

Open the org to the url of the jasmine tests:
sfdx force:org:open -u dap -p /c/jasmineTests.app
