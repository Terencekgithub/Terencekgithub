# Task 2: Installing and Configuring NGINX
# Connect to the VM using SSH
ssh <your_username>@<your_vm_public_ip>

# Install NGINX
sudo apt-get update
sudo apt-get install -y nginx

# Create a directory and a basic webpage
sudo mkdir /var/www/html/labs
sudo chown -R $USER /var/www/html/labs
ln -s /var/www/html/labs ~/html
echo "Hello from NGINX on Azure!" > ~/html/index.html
