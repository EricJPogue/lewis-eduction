# Lewis Education

[Azure Static Web Apps](https://docs.microsoft.com/azure/static-web-apps/overview) allows you to easily build [React](https://reactjs.org/) apps in minutes. Use this repo with the [React quickstart](https://docs.microsoft.com/azure/static-web-apps/getting-started?tabs=react) to build and customize a new static site.

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

# Deploy to Azure

az group create \
    --name lewis-eduction-test-rg \
    --location "eastus2"
    
az staticwebapp create \
    --name lewis-eduction-test \
    --resource-group lewis-eduction-test-rg \
    --source https://github.com/LewisEducation/lewis-eduction \
    --location "eastus2" \
    --branch main \
    --app-location "src" \
    --login-with-github


Last updated: Tuesday, August 8 at 12:03 pm.
