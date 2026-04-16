# BookShoppingCartMvc (A basic e-comm system for beginners)📚🛒

Initially it is designed to explain how shopping cart 🛒 works in dot net core mvc. But now it has more features except payment gateway. A ⭐ in repository is highly appreciated, helps to promote my content.

📢 Initially , this project was built with `.net 7` and `sql server 2022`. But it is `Upgraded to .net 10.0` and `sql server 2025` 

## Tech stack 🧑‍💻

   - Dotnet core mvc (.Net 10.0)
   - MS SQLServer 2025 (Database)
   - Entity Framework Core (ORM)
   - Identity Core (Authentication)
   - Bootstrap 5 (frontend)

## Tools I have used and their alternative (Updated versions)

- Visual Studio 2026 (Alternatives : .NET SDK + VS Code or .NET SDK + JetBrains Rider).
- Microsoft Sql Server Management Studio (Alternative : mssql extension for vscode / dbeaver).
- Instead of manually installing `sql server`, you can also used `sql server` which is spun up in `docker`.

**Note:** Every tool and tech is free for personal use. 

## How to run the project?🌐

### 1. With docker compse (Quickest way)

It is the quickest way to run the application. You don't need to install anything on your system, except docker. Make sure you have installed `Docker` in your machine. Now, run the following command

```bash
docker compose up -d
```

- Your application will be served at `http://localhost:8080/`.
- Admin's `username` and `password` is given below (How to logged-in with admin account??🧑‍💻🧑‍💻).

**Note:** If you want to debug application and want to modify the project, I would recommend to follow the second approach.

### 2. Manually setup every thing (Recommended for developers)

Make sure:
- Either Dotnet sdk 10.0 or VisualStudio 2026 pre-installed in your machine
- pre-installed Sql server 2025 or spun up it in docker container




. Open `appsettings.json` file and update connection string.

```json
"ConnectionStrings": {
  "conn": "data source=your_server_name;initial catalog=MovieStoreMvc; integrated security=true;encrypt=false"
}
```

**Note:** It is not mandatory to install `sql server 2025` in your machine. You can spin up the `sql server` in docker container and use that for this application. But in this case your connection string will be different `Server=localhost,1433;Database=BookShoppingCartMvc;User Id=sa;Password=your_password;TrustServerCertificate=True`.

 Run the project.

📢 When you run the project for the first time, it will do following things:

- It will generate the database
- It will seed some data
- It will create an account for `admin`

## How to logged-in with admin account?? 🧑‍💻🧑‍💻

Click on the link named `login` and get logged-in with these credentials.

```text
username: admin@gmail.com

password: Admin@123
```

## Thanks

If you find this repository useful, then consider to leave a ⭐.
