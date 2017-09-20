---
title: Installing Lightning Testing Service
layout: post
comments: true
published: true
---

Before tests can be written that will validate the Lightning components in the Dreamhouse app, the new framework needs to be installed.

If the Dreamhouse app has not yet been installed into a scratch org, see [Dreamhouse App in a scratch org]({% post_url 2017-09-19-dreamhouseapp-testing %} )

To install the Lightning Testing Service, either install via the package, or from source.

## Via package

Install the v1.1 package from [Lightning Testing Service Github](https://github.com/forcedotcom/LightningTestingService/releases).  The [LTS with Examples](https://test.salesforce.com/packaging/installPackage.apexp?p0=04tJ0000000EbBy) package was used in this example.

```
sfdx force:package:install -i 04tJ0000000EbBy  -u dap
```


## From source

Clone the git repository
```
git clone https://github.com/forcedotcom/LightningTestingService.git
```

Enter the code directory
```
cd LightningTestingService    
```




Once the testing framework is installed in the scratch org, browse to the url of the jasmine tests:

```
sfdx force:org:open -u dap -p /c/jasmineTests.app
```

Or run the tests through the CLI

```
sfdx force:lightning:test:run -u dap --appname jasmineTests.app
```

Note that if this command is run without supplying app name, by default the CLI will attempt to open Tests.app which does not exist in the github repository.