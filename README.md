Toy application for kicking the tires on ASP.NET core using VS Code.

Generated using [Yeoman aspnet generator](https://docs.microsoft.com/en-us/aspnet/core/client-side/yeoman) (yo aspnet)

* [Getting started with ASP.NET Core MVC and Entity Framework Core](https://docs.microsoft.com/en-us/aspnet/core/data/ef-mvc/intro)
* [Contoso University ASP.NET Core Source Code (Visual Studio)](https://github.com/aspnet/Docs/tree/master/aspnetcore/data/ef-mvc/intro/samples/cu-final)
* [Dotnet EF Migrations For ASP.NET Core](http://benjii.me/2016/05/dotnet-ef-migrations-for-asp-net-core/)
* [Adding EF Core and PostgreSQL to an ASP.NET Core project on OS X](http://andrewlock.net/adding-ef-core-to-a-project-on-os-x/)

Default configuration connects to Postgres on localhost via 127.0.0.1 (to get username / password authentication), using credentials username: aspnet_user password: dotnetrocks. The aspnet_user needs permission to create DBs and alter schema. 

Setup

git clone https://github.com/jerometerry/aspnetcoretoy.git

cd ./aspnetcoretoy/App

dotnet restore

bower install

dotnet ef database update --context ApplicationDbContext

dotnet ef database update --context SchoolContext 

dotnet run
