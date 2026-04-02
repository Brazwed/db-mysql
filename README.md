# db-mysql

MySQL 8 Docker container pre-configured.

## Option 1: Use with Database Toolkit (Recommended)

```bash
git clone --recurse-submodules https://github.com/Brazwed/Database.git
cd Database
sudo ./setup.sh install mysql
```

## Option 2: Standalone with Docker Compose

```bash
git clone https://github.com/Brazwed/db-mysql.git
cd db-mysql
cp .env.example .env
docker compose up -d
```

## Default Connection

```
Host:     localhost
Port:     3306
User:     mysql_user
Pass:     mysql_dev_2026
Database: devdb

mysql -h localhost -P 3306 -u mysql_user -pmysql_dev_2026 devdb
```

## Configuration

Edit `.env`:

```env
MY_USER=mysql_user
MY_PASS=mysql_dev_2026
MY_DB=devdb
MY_PORT=3306
```

## Part of Database Toolkit

https://github.com/Brazwed/Database
