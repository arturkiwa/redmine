Available environment variables:

##### User and Site configuration

- `REDMINE_PORT_NUMBER`: Port number in which Redmine will run. Default: **3000**
- `REDMINE_USERNAME`: Redmine application username. Default: **user**
- `REDMINE_PASSWORD`: Redmine application password. Default: **bitnami1**
- `REDMINE_EMAIL`: Redmine application email. Default: **user@example.com**
- `REDMINE_FIRST_NAME`: Redmine user first name. Default: **UserName**
- `REDMINE_LAST_NAME`: Redmine user last name. Default: **LastName**
- `REDMINE_LANGUAGE`: Redmine site default language. Default: **en**
- `REDMINE_REST_API_ENABLED`: Whether to allow REST API calls to Redmine. Default: **0**
- `REDMINE_LOAD_DEFAULT_DATA`: Whether to load default configuration data for Redmine. Default: **yes**
- `REDMINE_SKIP_BOOTSTRAP`: Whether to skip performing the initial bootstrapping for the application. This is necessary in case you use a database that already has Redmine data. Default: **no**

##### Database connection configuration

- `REDMINE_DATABASE_TYPE`: Database type to be used for the Redmine installation. Allowed values: *mariadb*, *postgresql*. Default: **mariadb**
- `REDMINE_DATABASE_HOST`: Hostname for the MariaDB or MySQL server. Default: **mariadb**
- `REDMINE_DATABASE_PORT_NUMBER`: Port used by the MariaDB or MySQL server. Default: **3306**
- `REDMINE_DATABASE_NAME`: Database name that Redmine will use to connect with the database. Default: **bitnami_redmine**
- `REDMINE_DATABASE_USER`: Database user that Redmine will use to connect with the database. Default: **bn_redmine**
- `REDMINE_DATABASE_PASSWORD`: Database password that Redmine will use to connect with the database. No default.
- `ALLOW_EMPTY_PASSWORD`: It can be used to allow blank passwords. Default: **no**

##### Create a MariaDB or MySQL database for Redmine using mysql-client

- `MYSQL_CLIENT_DATABASE_HOST`: Hostname for the MariaDB or MySQL server. Default: **mariadb**
- `MYSQL_CLIENT_DATABASE_PORT_NUMBER`: Port used by the MariaDB or MySQL server. Default: **3306**
- `MYSQL_CLIENT_DATABASE_ROOT_USER`: Database admin user. Default: **root**
- `MYSQL_CLIENT_DATABASE_ROOT_PASSWORD`: Database password for the database admin user. No default.
- `MYSQL_CLIENT_CREATE_DATABASE_NAME`: New database to be created by the mysql client module. No default.
- `MYSQL_CLIENT_CREATE_DATABASE_USER`: New database user to be created by the mysql client module. No default.
- `MYSQL_CLIENT_CREATE_DATABASE_PASSWORD`: Database password for the `MYSQL_CLIENT_CREATE_DATABASE_USER` user. No default.
- `MYSQL_CLIENT_CREATE_DATABASE_CHARACTER_SET`: Character set to use for the new database. No default.
- `MYSQL_CLIENT_CREATE_DATABASE_COLLATE`: Database collation to use for the new database. No default.
- `MYSQL_CLIENT_ENABLE_SSL`: Whether to enable SSL connections for the new database. Default: **no**
- `MYSQL_CLIENT_SSL_CA_FILE`: Path to the SSL CA file for the new database. No default.
- `ALLOW_EMPTY_PASSWORD`: It can be used to allow blank passwords. Default: **no**

##### Create a PostgreSQL database for Redmine using postgresql-client

- `POSTGRESQL_CLIENT_DATABASE_HOST`: Hostname for the PostgreSQL server. Default: **postgresql**
- `POSTGRESQL_CLIENT_DATABASE_PORT_NUMBER`: Port used by the PostgreSQL server. Default: **5432**
- `POSTGRESQL_CLIENT_POSTGRES_USER`: Database admin user. Default: **root**
- `POSTGRESQL_CLIENT_POSTGRES_PASSWORD`: Database password for the database admin user. No defaults.
- `POSTGRESQL_CLIENT_CREATE_DATABASE_NAME`: New database to be created by the mysql client module. No defaults.
- `POSTGRESQL_CLIENT_CREATE_DATABASE_USER`: New database user to be created by the mysql client module. No defaults.
- `POSTGRESQL_CLIENT_CREATE_DATABASE_PASSWORD`: Database password for the `POSTGRESQL_CLIENT_CREATE_DATABASE_USER` user. No defaults.
- `POSTGRESQL_CLIENT_CREATE_DATABASE_EXTENSIONS`: PostgreSQL extensions to enable in the specified database during the first initialization. No defaults.
- `ALLOW_EMPTY_PASSWORD`: It can be used to allow blank passwords. Default: **no**

##### SMTP Configuration

To configure Redmine to send email using SMTP you can set the following environment variables:

- `REDMINE_SMTP_HOST`: SMTP host.
- `REDMINE_SMTP_PORT`: SMTP port.
- `REDMINE_SMTP_USER`: SMTP account user.
- `REDMINE_SMTP_PASSWORD`: SMTP account password.
- `REDMINE_SMTP_PROTOCOL`: If specified, SMTP protocol to use. Allowed values: *tls*, *ssl*. No default.
- `REDMINE_SMTP_AUTH`: SMTP authentication method. Allowed values: *login*, *plain*, *cram_md5*. Default: **login**.
:warning:
