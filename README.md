# TodoApi

### Les principes fondamentaux d’une API web avec ASP.NET Core.

API web qui peut gérer des tâches stockées dans une base de données.

## Prérequis

```
dotnet add package Microsoft.EntityFrameworkCore.InMemory
dotnet add package Microsoft.VisualStudio.Web.CodeGeneration.Design
dotnet add package Microsoft.EntityFrameworkCore.Design
dotnet tool install -g dotnet-aspnet-codegenerator
dotnet tool update -g dotnet-aspnet-codegenerator
dotnet aspnet-codegenerator controller -name TodoItemsController -async -api -m TodoItem -dc TodoContext -outDir Controllers
```

## Apis

`GET /api/TodoItems`	     Obtenir toutes les tâches

`GET /api/TodoItems/{id}`	 Obtenir un élément par ID

`POST /api/TodoItems`	     Ajouter un nouvel élément

`PUT /api/TodoItems/{id}`	 Mettre à jour un élément existant

`DELETE /api/TodoItems/{id}` Supprimer un élément
