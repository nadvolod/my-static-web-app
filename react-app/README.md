# Static Web App

This project was created to help represent a fundamental app written with React. The shopping theme is used throughout the app.

## Getting Started

1. Create a repository from this template repository <https://github.com/MicrosoftDocs/mslearn-staticwebapp/generate>

1. Enter the name of your new repository as _my-static-web-app_

1. Clone your new repository

   ```bash
   git clone https://github.com/your-github-organization/my-static-web-app
   cd my-static-web-app/react-app
   ```

1. Install the npm packages

   ```bash
   npm install
   ```

1. Run the app

   ```bash
   npm start
   ```

1. Run the API

   ```bash
   cd api
   func start
   ```

API typically opens on http://localhost:7071/api/products and reads from `../api/shared/products-data.js`

## Troubleshooting

### Azure Sandbox for coding

Once you create a Sandbox, use it until you finish a module. Otherwise, you will need to restart 
from [here](https://docs.microsoft.com/en-us/learn/modules/publish-static-web-app-api-preview-url/2-exercise-get-started?pivots=react)

### Error: Missing binding

```text
Failed to compile.

./src/styles.scss (./node_modules/css-loader/dist/cjs.js??ref--6-oneOf-5-1!./node_modules/postcss-loader/src??postcss!./node_modules/resolve-url-loader??ref--6-oneOf-5-3!./node_modules/sass-loader/dist/cjs.js??ref--6-oneOf-5-4!./src/styles.scss)
Error: Missing binding /Users/nikolay/Documents/source/js/my-static-web-app/react-app/node_modules/node-sass/vendor/darwin-x64-83/binding.node
Node Sass could not find a binding for your current environment: OS X 64-bit with Node.js 14.x

Found bindings for the following environments:
  - OS X 64-bit with Node.js 12.x

This usually happens because your environment has changed since running `npm install`.
Run `npm rebuild node-sass` to download the binding for your current environment.
```

The code doesn't work with Node 15 and needs at max Node 14. 
Need to use NVM to install Node 14 and set it to default by using the answers [here](https://stackoverflow.com/questions/44700432/visual-studio-code-to-use-node-version-specified-by-nvm/66120222#66120222)

### Create Staging URL

the GitHub bot adds a comment to your pull request, which contains the URL of the pre-production environment. You can click on this link to see your staged changes.

### Constraints of Azure Static Apps API
Azure Static Web Apps provides an API through Azure Functions. The capabilities of Azure Functions are focused to a specific set of features that enable you to create an API for a web app and allow the web app to connect to API securely. These features come with some constraints, including:

The API route prefix must be api.
The API must either be a JavaScript, C#, or Python Azure Functions app.
Route rules for API functions only support redirects and securing routes with roles.
Triggers are limited to HTTP.
Input and output bindings are supported.
Logs are only available if you add Application Insights to your Functions app.

## Resources

### Azure Static Web Apps

- Learn how to [Publish an Angular, React, Svelte, or Vue JavaScript app and API with Azure Static Web Apps](https://docs.microsoft.com/learn/modules/publish-app-service-static-web-app-api?wt.mc_id=mslearn_staticwebapp-github-jopapa)
- [API support in Azure Static Web Apps](https://docs.microsoft.com/azure/static-web-apps/apis?wt.mc_id=mslearn_staticwebapp-github-jopapa)
- [Add an API to Azure Static Web Apps](https://docs.microsoft.com/azure/static-web-apps/add-api?wt.mc_id=mslearn_staticwebapp-github-jopapa)
- [Authentication and authorization](https://docs.microsoft.com/azure/static-web-apps/authentication-authorization?wt.mc_id=mslearn_staticwebapp-github-jopapa)
- [Routes](https://docs.microsoft.com/azure/static-web-apps/routes?wt.mc_id=mslearn_staticwebapp-github-jopapa)
- [Review pre-production environments](https://docs.microsoft.com/azure/static-web-apps/review-publish-pull-requests?wt.mc_id=mslearn_staticwebapp-github-jopapa)

### Azure Functions

- Learn how to [Refactor Node.js and Express APIs to Serverless APIs with Azure Functions](https://docs.microsoft.com/learn/modules/shift-nodejs-express-apis-serverless/?wt.mc_id=mslearn_staticwebapp-github-jopapa)
- Learn about the Azure Functions [local.settings.json](https://docs.microsoft.com/azure/azure-functions/functions-run-local#local-settings-file?wt.mc_id=mslearn_staticwebapp-github-jopapa) file
- Learn how to [Deploy to Azure Using Azure Functions](https://code.visualstudio.com/tutorials/functions-extension/getting-started?wt.mc_id=mslearn_staticwebapp-github-jopapa)
- Sign up for a [Free Trial of Azure](https://azure.microsoft.com/free/?wt.mc_id=mslearn_staticwebapp-github-jopapa)

### Visual Studio Code

- [Azure Free Trial](https://azure.microsoft.com/free/?wt.mc_id=mslearn_staticwebapp-github-jopapa)
- [VS Code](https://code.visualstudio.com?wt.mc_id=mslearn_staticwebapp-github-jopapa)
- [VS Code Extension for Node on Azure](https://marketplace.visualstudio.com/items?itemName=ms-vscode.vscode-node-azure-pack&WT.mc_id=mslearn_staticwebapp-github-jopapa)
- Azure Functions [local.settings.json](https://docs.microsoft.com/azure/azure-functions/functions-run-local#local-settings-file?WT.mc_id=mslearn_staticwebapp-github-jopapa) file

### Debugging Resources

- [Debugging Angular in VS Code](https://code.visualstudio.com/docs/nodejs/angular-tutorial?wt.mc_id=mslearn_staticwebapp-github-jopapa)
- [Debugging React in VS Code](https://code.visualstudio.com/docs/nodejs/reactjs-tutorial?wt.mc_id=mslearn_staticwebapp-github-jopapa)
- [Debugging Vue in VS Code](https://code.visualstudio.com/docs/nodejs/vuejs-tutorial?wt.mc_id=mslearn_staticwebapp-github-jopapa)
