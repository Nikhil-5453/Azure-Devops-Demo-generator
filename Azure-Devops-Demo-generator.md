Azure-Devops-Demo-generator



Pre-requitses:

\-> Install C# Dev kit, .Net install tool in VS code.

\-> Install dotnet8.0 sdk; 

&#x20;  for my system installed *dotnet-sdk-8.0.425-win-x64.exe*

\-> Verify: 

&#x20;    dotnet --list-sdks

&#x20;    dotnet --list-runtimes
-> Check for any vulenrabilites
   dotnet list package --vulnerable

project steps:

\-> Go to Azure-DevOps-Demo-generator and clone that repo.


\-> update the "Subscription id" of Azure Portal account in <AzDevOpsDemoGenerator/src/ADOGenerator/appsettings.json> in feild of 'scopes'

-> Go to path <AzDevOpsDemoGenerator/src/ADOGenerator/> In here we have project file 'ADOGenerator.csproj'

-> Build the Application: dotnet build ADOGenerator.csproj

-> Now run the application: dotnet run --project ADOGenerator.csproj

-> I choose 'eShopOnWeb' and 'PartsUnlimited' project Templates.

-> It will ask authentication method, I Choose PAT token
   Generate PAT in Azure portal under 'user-settings' and paste in here.

-> This will create projects in Azure DevOps portal.



