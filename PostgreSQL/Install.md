# Install

## 1. Official Website

https://www.postgresql.org/download/macosx/

[Download the installer](https://www.enterprisedb.com/downloads/postgres-postgresql-downloads)

Installation Directory: /Library/PostgreSQL/16

Data Directory: /Library/PostgreSQL/16/data

User: postgres

Port: 5432

## Start/Stop PostgreSQL

pg_ctl don't allow the root user to execute the commands.

```bash
sudo su - postgres # change user
cd /Library/PostgreSQL/16/bin
./pg_ctl restart -D /Library/PostgreSQL/16/data
```