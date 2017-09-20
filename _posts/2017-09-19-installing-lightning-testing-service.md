---
title: Installing Lightning Testing Service
layout: post
comments: true
published: true
---

Before tests can be written that will validate the Lightning components in the Dreamhouse app, the new framework, the new framework needs to be installed.

If the Dreamhouse app has not yet been installed into a scratch org, see [Dreamhouse App in a scratch org]({{ post_url 2017/09/19/dreamhouseapp-testing.html}} )

Install the v1.1 package from [Lightning Testing Service Github](https://github.com/forcedotcom/LightningTestingService/releases).  The [LTS with Examples](https://test.salesforce.com/packaging/installPackage.apexp?p0=04tJ0000000EbBy) package was used in this example.
sfdx force:package:install -i 04tJ0000000EbBy  -u dap

Open the org to the url of the jasmine tests:
sfdx force:org:open -u dap -p /c/jasmineTests.app
