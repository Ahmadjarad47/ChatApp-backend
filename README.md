# ChatApp â€” Backend

Social chat application back end built with **ASP.NET Core 7**, Clean Architecture and CQRS.

## Features

- **Auth** â€” register, login, JWT tokens, ASP.NET Core Identity with roles
- **Members** â€” member list with filtering and pagination, profile updates
- **Photos** â€” upload, remove, set main photo
- **Likes** â€” like members and list likes
- **Messages** â€” send, read, list (inbox / outbox / thread) and delete messages
- **Admin** â€” manage user roles
- **Data seeding** â€” users, photos and messages

## Architecture

```
src/
â”œâ”€â”€ Core/            Application (commands, queries, DTOs, validators, mapping) آ· Domain (entities)
â”œâ”€â”€ Infrastructure/  Persistence (EF Core, repositories, seeding)
â””â”€â”€ Presentation/    ChatApp.API (controllers, Swagger)
```

## Tech Stack

.NET 7 آ· MediatR (CQRS) آ· FluentValidation آ· AutoMapper آ· Entity Framework Core (SQL Server) آ· ASP.NET Core Identity آ· JWT آ· Swagger

## Getting Started

**Prerequisites:** .NET 7 SDK, SQL Server.

```bash
git clone https://github.com/Ahmadjarad47/ChatApp-backend.git
cd ChatApp-backend
# set the connection string and token key in appsettings.Development.json
dotnet restore
dotnet run --project src/Presentation/ChatApp.API
```

## Author

**Ahmad Jarad** â€” [GitHub](https://github.com/Ahmadjarad47)