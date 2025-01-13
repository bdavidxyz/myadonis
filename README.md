# Jumpstart AdonisJS 6

## Prerequisites

```bash
nodejs version : 22
git version 2.46.0
PostgreSQL version : 17.2
```

## Install a local DB

Open SQL CLI

- Linux or mac: `sudo -u postgres psql`
- Windows: `psql -U postgres`

Windows or Linux: you will need to provide the password set during the installation unless you ran it as an administrator.

```sql
CREATE DATABASE db_myadonis;
CREATE USER user_myadonis WITH SUPERUSER PASSWORD 'password';
GRANT ALL PRIVILEGES ON DATABASE db_myadonis TO user_myadonis;
ALTER DATABASE db_myadonis OWNER TO user_myadonis;

```

## Install env var

copy .env.example into .env

## Install project locally

```shell
npm install
node ace migration:run
node ace db:seed
npm run dev
```

## Access the project on your local Server

Once the server is running, open your browser and navigate to:

<http://localhost:3333>

