"# Azure_steveEV" 

Run steveev in Azure:
1. Create resource group: az group create --name steveevGroup --location "South Central US"
2. create app service plan: az appservice plan create --name steveevPlan --resource-group steveevGroup  --sku S1 --is-linux
3. create docker compose plan: az webapp create --resource-group steveevGroup --plan steveevPlan --name steve --multicontainer-config-type compose --multicontainer-config-file docker-compose.yml


##todo:

Add this in devops
