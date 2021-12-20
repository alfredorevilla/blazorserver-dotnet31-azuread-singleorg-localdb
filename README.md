# ClaimsPrincipal.IsInRole(string) sample

## Setup
- [.NET 3.1](https://dotnet.microsoft.com/en-us/download/dotnet/3.1).
- [Get an Azure AD tenant](https://docs.microsoft.com/en-us/azure/active-directory/develop/quickstart-create-new-tenant)
- [Register a Single Page Application in Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/develop/scenario-spa-app-registration) using the following parameters:  
  - Enable implicit grant flow for `id_token`
  - Redirect URIs:
    - https://localhost:44373/ 
    - https://localhost:5001
- [Create an application role](https://docs.microsoft.com/en-us/azure/active-directory/develop/howto-add-app-roles-in-azure-ad-apps) named `Admin` for users.
- [Assign the desired users to the previously created application role](https://docs.microsoft.com/en-us/azure/active-directory/develop/howto-add-app-roles-in-azure-ad-apps#assign-users-and-groups-to-roles).
- [Update your .NET application `AzureAd` section values](https://docs.microsoft.com/en-us/azure/active-directory/develop/scenario-web-app-sign-user-app-configuration?tabs=aspnetcore#configuration-files) with the propers ones from your Azure AD tenant and app registration.

## Run
- From command line execute:
  ```bash
  dotnet start
  ```

- From Visual Studio: Press `CTRL+F5`

## Motivation
https://docs.microsoft.com/en-us/answers/questions/665200/user-roles.html

## Additional Reference:
https://docs.microsoft.com/en-us/dotnet/api/system.security.claims.claimsprincipal.isinrole?view=netcore-3.1



