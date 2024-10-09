How to install : # Install the required dependencies
sudo apt install wget ca-certificates

# Add the pgAdmin repository
wget --quiet -O - https://www.pgadmin.org/static/packages_pgadmin_org.pub | sudo tee /etc/apt/trusted.gpg.d/pgadmin.asc

# Add the pgAdmin repository to the APT sources list
sudo sh -c 'echo "deb https://ftp.postgresql.org/pub/pgadmin/pgadmin4/apt/jammy pgadmin4 main" > /etc/apt/sources.list.d/pgadmin4.list && apt update'

# Install pgAdmin
sudo apt install pgadmin4
