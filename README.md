# db-mysql

MySQL 8 Docker container pre-configured. Ready to use, zero conflicts.

## Quick Start

```bash
git clone https://github.com/Brazwed/db-mysql.git
cd db-mysql
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

Edit `.env` (created automatically from `.env.example`):

```env
MY_USER=mysql_user
MY_PASS=mysql_dev_2026
MY_DB=devdb
MY_PORT=3306
```

## Part of Database Toolkit

This repo can be used standalone or with other databases via [Database Toolkit](https://github.com/Brazwed/Database).
