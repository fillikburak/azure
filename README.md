- Set-ExecutionPolicye Unrestricted
- az login
- az group list -o yaml
- az group create --name rg-buraktest1 --location westeurope
- az group list -o table
- az vm create --name burakvm1 --resource-group rg-buraktest1 --image Win2019Datacenter --size Standard_B1s

Azure Powershell
- Install-Module -Name Az -Repository PSGallery -Force
- -DeviceCode if browser not supported
- Connect-AzAccount
- Get-AzResourceGroup
- Get-AzResourceGroup | ConvertTo-Json
- Get-AzResourceGroup | Select-Object Location
- New-AzResourceGroup -Name buraktest2 -Location northeurope
- New-AzVM -Name burakvm2 -Location northeurope -Size Standard_B1s -Image Win2019Datacenter
