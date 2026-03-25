# Reference: https://hub.docker.com/_/mysql
# We use MySQL 8.0 to match what vProfile expects.
FROM mysql:8.0

# These environment variables configure the database
ENV MYSQL_ROOT_PASSWORD="admin123"
ENV MYSQL_DATABASE="accounts"
ENV MYSQL_USER="admin"
ENV MYSQL_PASSWORD="admin123"

# Seed the database with initial data
COPY db_backup.sql /docker-entrypoint-initdb.d/db_backup.sql

# MySQL default port
EXPOSE 3306
