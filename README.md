# db-mysql

MySQL 8 Docker container pré-configurado. Pronto pra usar, sem conflitos.

## Uso rápido

```bash
git clone https://github.com/Brazwed/db-mysql.git
cd db-mysql
docker compose up -d
```

## Conexão padrão

```
Host:     localhost
Porta:    3306
Usuário:  mysql_user
Senha:    mysql_dev_2026
Banco:    devdb

mysql -h localhost -P 3306 -u mysql_user -pmysql_dev_2026 devdb
```

## Configuração

Edite `.env` (criado automaticamente de `.env.example`):

```env
MY_USER=mysql_user
MY_PASS=mysql_dev_2026
MY_DB=devdb
MY_PORT=3306
```

## Parte do Database Toolkit

Este repositório pode ser usado standalone ou junto com outros bancos via [Database](https://github.com/Brazwed/Database).
