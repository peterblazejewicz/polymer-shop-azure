# SHOP

### Setup

##### Prerequisites

Install [polymer-cli](https://github.com/Polymer/polymer-cli):
(Need at least npm v0.3.0)

    npm install -g polymer-cli


##### Setup
    # Using CLI
    mkdir shop
    cd shop
    polymer init shop
    
    # Or cloning direct from GitHub
    git clone https://github.com/Polymer/shop.git
    cd shop
    bower install

### Generate Azure deployment script

This was done using [Azure xplat cli](https://github.com/Azure/azure-xplat-cli)

> NOTE: https://github.com/Azure/azure-xplat-cli/issues/3245

```bash
azure site deploymentscript --aspNetCore ./project.json
```

### Start the development server

    polymer serve

### Run web-component-tester tests

    polymer test

### Build

    polymer build

### Test the build

This command serves the minified version of the app in an unbundled state, as it would be served by a push-compatible server:

    polymer serve build/unbundled
    
This command serves the minified version of the app generated using fragment bundling:

    polymer serve build/bundled

## Deployment to Azure

### Create Azure web site

[Create a web app in an App Service Environment](https://azure.microsoft.com/en-us/documentation/articles/app-service-web-how-to-create-a-web-app-in-an-ase/)

### Configure Web App

#### Configure NodeJS version

```ini
WEBSITE_NODE_DEFAULT_VERSION = 6.7.0
```
#### Configure private extensions

```ini
WEBSITE_PRIVATE_EXTENSIONS = 1
```

#### Install Yarn and Polymer CLI tools

[azure-site-extensions](https://github.com/peterblazejewicz/azure-site-extensions)

### Deploy your web application

Now you can deploy your application using Azure deployment integration with Git local or Github repository:

[Automating code deployment with GitHub and Azure](https://github.com/blog/2056-automating-code-deployment-with-github-and-azure)

## Author

@peterblazejewicz
