## [Capture Web App Logs with App Service Diagnostic Logging](https://docs.microsoft.com/en-nz/learn/modules/capture-application-logs-app-service/?WT.mc_id=cloudskillschallenge_8351edfe-a67a-46d4-81cd-6439844b72ac&ns-enrollment-type=Collection&ns-enrollment-id=67pku71drej4)
* Only Windows apps can save logs to Azure storage
* File system logs are rotated after 24 hours for performance
* Deploy an Azure Web App...
```bash
az appservice plan create --name $appPlan --resource-group $resourceGroup --location $appLocation --sku FREE

az webapp create --name $appName --resource-group $resourceGroup --plan $appPlan --deployment-source-url $gitRepo

az storage account create -n $storageAccount -g $resourceGroup -l $appLocation --sku Standard_LRS
```
* Tail logs...
```bash
az webapp log tail --name contosofashions1223 --resource-group learn-1f9306f6-00ed-44c7-8f5b-beb1670acc5c
```
* Can also view logs with curl and some weird ftps credentials
* Download logs...
```bash
az webapp log download --log-file contosofashions.zip  --resource-group learn-1f9306f6-00ed-44c7-8f5b-beb1670acc5c --name contosofashions1223
```
* Can also use some weird stuff called [Kudu](https://github.com/projectkudu/kudu/wiki) to download logs
* Or even Storage Explorer
