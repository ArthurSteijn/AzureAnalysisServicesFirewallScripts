# AzureAnalysisServicesFirewallScripts
Scripts for managing Azure Analysis Services Firewall configs

Azure Analysis Services has [basic firewall capabilities](https://azure.microsoft.com/en-us/blog/hardening-azure-analysis-services-with-the-new-firewall-capability/).  
When new versions of models are deployed through Azure DevOps, the IP Address of the Agent needs to be added to the Firewall Config. 

The PowerShell script *'AddDevOpsIpToAAS.ps1'* adds a new Firewall Rule with the current IP Address to the Config

The *'AddDevOpsIpToAAS.ps1'* script can be used in an Azure DevOps pipeline to add the IP Address of the Agent  
that performs the deployment of the Azure Analysis Services model on the server. 

The *'AddDevOpsIpToAAS.yml'* file is an example of how to incorperate the PowerShell script into an Azure Pipeline. 