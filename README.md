# Movie Managment System
This is a simple movie managment web app with persistency realised via ASP.NET Core MVC

# Technologies
Some of the technologies used in the project
- C#/NET
- ASP
- Entity Framework Core
- SQL Server
- REST API
- HTML/CSS

# How to Deploy from source
## Requirements:
- .NET >= 8.0.401
- Entity Framework Core >= 9.0.0
- Sql Server 2022

## Before running
- You should have [SQL Server](https://www.microsoft.com/en-us/sql-server/sql-server-downloads) running and modify server url, username and password in [appsettings.json](appsettings.json) accordingly
- Build migration: `dotnet ef migrations add InitialCreate`
- Apply migration to the database: `dotnet ef database update`

## Run the web app:
You can run the web app by executing `dotnet run` command in root directory of the project.

# How to Deploy from docker
## Export enviroment variables 
export ConnectionStrings__mvcmoviecontext="[ Connection String ]"

```docker
docker pull warmek/movie-managment-system
```
