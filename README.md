# SqlSyringe.Practice.Core3
A practice demo for SqlSyringe, using .NET Core -3.0-  2.2

Run it locally:

Ubuntu:

- git clone https://github.com/suterma/SqlSyringe.Practice.Core3.git
- dotnet build
- Create the database: `dotnet ef database update` OR `Update-Database` in the Package Manager Console
- dotnet run
- Browse to the indicated URL, e.g. https://localhost:5001
- Click on the SqlSyringe link



Example Queries:

Get all Tables:
SELECT TABLE_NAME FROM INFORMATION_SCHEMA.TABLES WHERE TABLE_TYPE='BASE TABLE'

//TODO pending
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


