# ⚙️ Create & Run a .NET Web API using Bash

This guide shows how to **create, run, and test a new Web API project** using the command line (bash) with **C# and .NET**.

---

# 🚀 Prerequisites

Make sure you have installed:

* .NET SDK (check with `dotnet --version`)
* A terminal (Git Bash, WSL, or Linux/Mac terminal)

---

# 🏗️ 1. Create a New Web API Project

```bash id="a1b2c3"
dotnet new webapi -n MyWebApi
```

👉 This creates a new project folder:

```id="d4e5f6"
MyWebApi/
```

---

# 📂 2. Navigate into the Project

```bash id="g7h8i9"
cd MyWebApi
```

---

# 📦 3. Restore Dependencies

```bash id="j1k2l3"
dotnet restore
```

👉 Downloads all required packages

---

# ▶️ 4. Run the Application

```bash id="m4n5o6"
dotnet run
```

👉 You should see:

```id="p7q8r9"
Now listening on: https://localhost:XXXX
```

---

# 🌐 5. Open Swagger UI

Open your browser and go to:

```id="s1t2u3"
https://localhost:XXXX/swagger
```

👉 Replace `XXXX` with your port

---

# 🔧 Optional: Run on a Specific Port

```bash id="v4w5x6"
dotnet run --urls "http://localhost:5000"
```

Then open:

```id="y7z8a9"
http://localhost:5000/swagger
```

---

# 📦 6. Add Packages (Optional)

Example: Install Swagger manually

```bash id="b1c2d3"
dotnet add package Swashbuckle.AspNetCore
```

Example: Install Entity Framework

```bash id="e4f5g6"
dotnet add package Microsoft.EntityFrameworkCore.InMemory
```

---

# 🧪 7. Test the API

Use:

* Swagger UI (browser)
* curl (terminal)
* Postman

Example using curl:

```bash id="h7i8j9"
curl http://localhost:5000/weatherforecast
```

---

# 🧹 8. Useful Commands

Build project:

```bash id="k1l2m3"
dotnet build
```

Clean project:

```bash id="n4o5p6"
dotnet clean
```

List installed packages:

```bash id="q7r8s9"
dotnet list package
```

---

# 🧠 How It Works

1. `dotnet new webapi` → creates a REST API project
2. `dotnet run` → starts a local web server
3. Browser/Client → sends HTTP requests
4. API → processes and returns JSON responses

---
