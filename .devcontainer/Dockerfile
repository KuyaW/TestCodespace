# Use official PHP devcontainer image
FROM mcr.microsoft.com/vscode/devcontainers/php:8.1

# Install MySQL and required tools
RUN apt-get update && \
    DEBIAN_FRONTEND=noninteractive apt-get install -y mysql-server mysql-client && \
    apt-get clean && rm -rf /var/lib/apt/lists/*

# Start MySQL on container start
CMD ["bash", "-c", "service mysql start && tail -f /dev/null"]
