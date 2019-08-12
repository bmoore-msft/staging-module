# staging-module
Sample PS module for staging artifacts - prototype uses public storage

This shows a working prototype of staging artifacts to storage and authoring templates using relative references without a sasToken.  This is a prototype that uses public storage to show the sample code.

Import the PSM1 and then use the New-AzDeployment2 command to point to a folder to deploy a sample.

First:
```
Import-Module .\setup\Deploy-AzTemplate.psm1
```

Then:
```
New-AzDeployment2 -ArtifactsStagingDirectory .\contosportal -location westus2
```
