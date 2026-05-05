Cosmetic & Beauty Products Online Shop (cbpos)
⚠️ Note – The project was originally distributed as a zip file with a “Default Project” inside cbpos.zip.

This README describes how to set it up locally using XAMPP, import the database and get started.

## Table of Contents
1. [Prerequisites](#prerequisites)
2. [Installation & Setup](#installation--setup)
   - 2.1 [Download Source Code](#download-source-code)
   - 2.2 [Install XAMPP](#install-xampp)
   - 2.3 [Extract & Copy Files](#extract--copy-files)
   - 2.4 [Create Database](#create-database)
   - 2.5 [Import SQL Dump](#import-sql-dump)
   - 2.6 [Run the Application](#run-the-application)
3. [Login Credentials](#login-credentials)
4. [Project Structure](#project-structure)
5. [Contributing & Feedback](#contributing--feedback)
6. [License](#license)

---

## 1. Prerequisites

| Item | Version |
|------|---------|
| **PHP** | 7.4+ (XAMPP includes PHP) |
| **MySQL / MariaDB** | 5.7+ (XAMPP includes MySQL) |
| **Web Server** | Apache (included in XAMPP) |
| **Text Editor** | Notepad++, Sublime Text, VS Code … |

> *If you prefer Docker or another stack, adjust the steps accordingly.*

---

## 2. Installation & Setup

### 2.1 Download Source Code
```bash
# Clone the repo (or download ZIP and extract)
git clone https://github.com/Silent-Galaxy/ui_ux_FullShop.git cbpos
```

> The repository contains a `cms` folder that is the actual application.

### 2.2 Install XAMPP

1. Download [XAMPP](https://www.apachefriends.org/index.html) for your OS.  
2. Run the installer and install to **C:\xampp** (or any other drive).  
3. Start Apache & MySQL from the XAMPP Control Panel.

### 2.3 Extract & Copy Files

```bash
# Assuming you extracted cbpos.zip to a folder called `cbpos`
cd path/to/cbpos
cp -r cms/* /path/to/xampp/htdocs/
```

> *If you installed XAMPP on drive D or E, replace `/path/to/xampp` accordingly.*

### 2.4 Create Database

1. Open your browser → `http://localhost/phpmyadmin`.  
2. Click **New** → Name the database **cbpos_db** → Click **Create**.

### 2.5 Import SQL Dump

```bash
# From phpMyAdmin: choose cbpos_db, go to Import tab,
# select file `sql/cbpos_db.sql` (inside the repo) and import.
```

> The SQL file is located at `cbpos/sql/cbpos_db.sql`.

### 2.6 Run the Application

Open a browser and navigate to:

```
http://localhost/cbpos
```

You should see the home page of the online shop.

---

## 3. Login Credentials

| Role   | Username | Password |
|--------|----------|----------|
| Admin  | admin    | admin123 |
| User   | (create your own) | — |

> After logging in as admin you can create regular users via the dashboard.

---

## 4. Project Structure

```
cbpos/
├─ cms/                # Core application files
│  ├─ assets/          # CSS, JS, images
│  ├─ includes/        # PHP includes (header, footer, etc.)
│  ├─ modules/         # Functional modules (products, cart, orders)
│  └─ index.php        # Front controller
├─ sql/
│   └─ cbpos_db.sql    # Database dump
└─ README.md           # This file
```

> *Feel free to explore the code – it’s a simple MVC‑style PHP app.*

---

## 5. Contributing & Feedback

- **Issues**: Report bugs or feature requests in GitHub Issues.
- **Pull Requests**: Fork, make changes, and submit a PR.
- **Discord**: Join the community at <https://discord.gg/2jDAHeqXeQ>.

---

## 6. License

MIT © SilentGalaxy  
(See `LICENSE` file)

--- 

### Screenshots (for reference)

*(The original post contained many screenshots; they are omitted here for brevity but can be found in the repository under `screenshots/`.)*


![image](https://github.com/Silent-Galaxy/ui_ux_FullShop/assets/91001518/b57db2bd-3354-4c12-be3d-631ab27549fa)
![image](https://github.com/Silent-Galaxy/ui_ux_FullShop/assets/91001518/a1e67250-a4f5-4835-95c6-88fca0f4b32e)
![image](https://github.com/Silent-Galaxy/ui_ux_FullShop/assets/91001518/ab34d8bc-6359-4dbb-868d-f9d0a7802dbc)
![image](https://github.com/Silent-Galaxy/ui_ux_FullShop/assets/91001518/70ee128a-3b75-49e4-8501-fc5370efb951)
![image](https://github.com/Silent-Galaxy/ui_ux_FullShop/assets/91001518/36d08a76-ff91-43f5-b3f4-53deedd2668e)
![image](https://github.com/Silent-Galaxy/ui_ux_FullShop/assets/91001518/b1c1dc36-6bc4-45e5-aec2-0bc9aa33a3ec)
![image](https://github.com/Silent-Galaxy/ui_ux_FullShop/assets/91001518/835deb24-261c-4889-9e32-fb558212f09f)
![image](https://github.com/Silent-Galaxy/ui_ux_FullShop/assets/91001518/96b0c874-1363-4c2a-bfe7-248c373ad190)
![image](https://github.com/Silent-Galaxy/ui_ux_FullShop/assets/91001518/185b5f7f-b430-4b67-a2be-529ecc4e4d26)
![image](https://github.com/Silent-Galaxy/ui_ux_FullShop/assets/91001518/e0eae230-3fb8-4df9-a30f-6d655cc9a601)
![image](https://github.com/Silent-Galaxy/ui_ux_FullShop/assets/91001518/006a792a-abe2-485b-b602-6f4f6081fb7f)
![image](https://github.com/Silent-Galaxy/ui_ux_FullShop/assets/91001518/d4a20224-ceaf-4746-b059-2b2a357c2cfc)
![image](https://github.com/Silent-Galaxy/ui_ux_FullShop/assets/91001518/ed7eb015-b34c-4f72-98b2-1fa5f63e9191)
![image](https://github.com/Silent-Galaxy/ui_ux_FullShop/assets/91001518/f23018eb-08ed-4d17-a4cd-c58529946253)
![image](https://github.com/Silent-Galaxy/ui_ux_FullShop/assets/91001518/26616565-93c9-453b-b0e2-189f21c8e08c)
![image](https://github.com/Silent-Galaxy/ui_ux_FullShop/assets/91001518/6b9e8aea-a4d6-407d-b773-d572f5dcfe04)
![image](https://github.com/Silent-Galaxy/ui_ux_FullShop/assets/91001518/c7e1ab24-e43f-489b-9fda-f318dbd3de37)

---

**Happy coding!**

> *If you need Persian localisation or ZarinPal integration, keep an eye on future releases.*
