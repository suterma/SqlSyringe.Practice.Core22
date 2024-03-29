# SqlSyringe.Practice.Core22
A practice demo for [SqlSyringe](https://github.com/suterma/SqlSyringe), using .NET Core 2.2, for running locally with a [SQL Server Express LocalDB](https://docs.microsoft.com/en-us/sql/database-engine/configure-windows/sql-server-express-localdb?view=sql-server-ver15)

## Run on Windows

- Clone this repository (e.g. using the [GitHub Desktop](https://desktop.github.com/) or the [Git For Windows](https://gitforwindows.org/) client)
- In Visual Studio 2019, open the solution
- Create the database: on the command line, run `dotnet ef database update` or in Visual Studio 2019, run `Update-Database` in the Package Manager Console
- Build and run the solution
- Click on the SqlSyringe link

## Run on Ubuntu

Since LocalDB is only available on Windows, you must create and configure an alternative database. 
On the command line
`git clone https://github.com/suterma/SqlSyringe.Practice.Core22.git`
Create and configure an alternative database
`dotnet build`
`dotnet run`
- Browse to the indicated URL, e.g. https://localhost:5001
- Click on the SqlSyringe link

## Deploy on Azure
Use this button to automatically deploy this web app as your own Azure App

<a href="https://azuredeploy.net/" target="_blank"><img src="http://azuredeploy.net/deploybutton.png"/></a>

## Example Queries:

Get all Tables: `SELECT TABLE_NAME FROM INFORMATION_SCHEMA.TABLES WHERE TABLE_TYPE='BASE TABLE'`

<!---
# Deploy on azure

To deploy on azure, go to 
 - https://azure.microsoft.com/en-us/try/app-service/web
 - select the ASP.NET Core Template, click Create

The web app is deployed for you

 - Go to "Edit your code online"
 - Remove all files and folder in WWWROOT, leaving just the emtpy folder
 - Select the GitHup icon on the left
 - Clone from this repo using it's URL
 - Look for the web console, until it reaches 100% checkout
 - Build using "dotnet build"
 - dotnet run (//TODO only works locally)
 - Hit the play button on the left
--->

