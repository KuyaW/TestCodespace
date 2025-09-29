# Base image
FROM mcr.microsoft.com/vscode/devcontainers/php:8.1

# Install MySQL
RUN apt-get update && apt-get install -y mysql-server

# Expose MySQL default port
EXPOSE 3306

# Start MySQL server in the background
CMD service mysql start && tail -f /dev/null
