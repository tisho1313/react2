# Azure Static Web Apps for Visual Studio Code



Use this extension to quickly create and manage Azure Static Web Apps directly from VS Code.

**Visit the [wiki](https://github.com/Microsoft/vscode-azurestaticwebapps/wiki) for additional information about the extension.**

> Sign up today for your free Azure account and receive 12 months of free popular services, $200 free credit and 25+ always free services 👉 [Start Free](https://azure.microsoft.com/free/open-source).

## Support for [vscode.dev](https://vscode.dev/)

The Azure Static Web Apps extension supports running on [vscode.dev](https://vscode.dev/) and [github.dev](http://github.dev/). Open a GitHub repository to create and update Static Web Apps directly from your browser! Debugging is not supported on the web. Note that this does not require the Azure Account extension and uses VS Code's built-in authentication provider.

## Run and debug your static web app

![Debug static web app with a dynamic configuration](https://github.com/Microsoft/vscode-azurestaticwebapps/raw/main/resources/readme/debugging.gif)

✨ Check out [Guide: Debugging a Static Web App with VS Code](https://aka.ms/setupSwaCliCode) for instructions and more information about debugging a static web app.

## Create your first static web app

1. Click the '+' button in the explorer to setup a new static web app

    ![Create Static Web App](https://github.com/Microsoft/vscode-azurestaticwebapps/raw/main/resources/readme/create_resource.png)

1. Select "Create Static Web App..."

    ![Create Static Web App](https://github.com/Microsoft/vscode-azurestaticwebapps/raw/main/resources/readme/create_swa.png)

1. Authorize access to your GitHub account so the extension can find your repositories

    ![Authorize Access to through GitHub](https://github.com/Microsoft/vscode-azurestaticwebapps/raw/main/resources/readme/authorize_access_github.png)

    ![Authorize Access to through GitHub](https://github.com/Microsoft/vscode-azurestaticwebapps/raw/main/resources/readme/authorize_access_github_2.png)
1. Select a repository and branch that will be deployed to the static web app
    > If your local project has a remote configured, the extension will default to that repository
1. Provide the app folder name
    > Location of your application code. For example, '/' represents the root of your app, while '/app' represents a directory called 'app'.
1. Provide the api folder name (optional)
    > Location of your Azure Functions code. For example, '/api' represents a folder called 'api'. If you don't have an Azure Functions project yet, don't worry!  This is optional so just leave this blank.
1. Provide the build artifact folder name
    > The path of your build output relative to your apps location. For example, setting a value of 'build' when your app location is set to '/app' will cause the content at '/app/build' to be served.

✨ [See recommended settings for popular frameworks and libraries](https://aka.ms/AAdb4fs)

## Updating your static web app

Commit and push your changes to the GitHub repository that your static web app is configured to.  It will then use [GitHub Actions](https://github.com/features/actions) to update your app.

If you create a pull request through GitHub, GitHub Actions will create a staging environment with your new changes live.  Your Production environment and staging environments are all listed within your Static Web App as well as application settings.

> **IMPORTANT:** The application settings only apply to the backend API of an Azure Static Web App.

![Static Web App Environments](https://github.com/Microsoft/vscode-azurestaticwebapps/raw/main/resources/readme/static_web_app_environments.png)

## Create a HTTP Function for your static web app

You can add a serverless API to your static web app by creating a HTTP Functions project.

1. Open your static web app project in your Visual Studio Code workspace
1. Select the button to create a new HTTP Function

    ![Create HTTP Function](https://github.com/Microsoft/vscode-azurestaticwebapps/raw/main/resources/readme/create_http_function.png)

1. Provide a HTTP Function name that is unique to your API
1. If this is your first HTTP Function, select a language for your API

![Select Language](https://github.com/Microsoft/vscode-azurestaticwebapps/raw/main/resources/readme/select_language.png)



## Telemetry

VS Code collects usage data and sends it to Microsoft to help improve our products and services. Read our [privacy statement](https://go.microsoft.com/fwlink/?LinkID=528096&clcid=0x409) to learn more. If you don’t wish to send usage data to Microsoft, you can set the `telemetry.enableTelemetry` setting to `false`. Learn more in our [FAQ](https://code.visualstudio.com/docs/supporting/faq#_how-to-disable-telemetry-reporting).

## License

[MIT](https://github.com/Microsoft/vscode-azurestaticwebapps/blob/main/LICENSE.md)
