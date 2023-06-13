# Setup Inicial Server Jenkins

- Setup resource Group basico.

# Script 

- criar arquivo cloud-init-jenkins.txt.

#cloud-config
package_upgrade: true
runcmd:
  - sudo apt install openjdk-11-jre -y
  - curl -fsSL https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key | sudo tee /usr/share/keyrings/jenkins-keyring.asc > /dev/null
  -  echo 'deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] https://pkg.jenkins.io/debian-stable binary/' | sudo tee /etc/apt/sources.list.d/jenkins.list > /dev/null
  - sudo apt-get update && sudo apt-get install jenkins -y
  - sudo service jenkins restart


 # Criar VM jenkins com 8gb ram

# VM com 2cpu e 8gb ran  ssd 1024gb armazenamento

az vm create \
--resource-group jenkins-get-started-rg \
--name jenkins-server-vm \
--image UbuntuLTS \
--data-disk-sizes-gb 1024 \
--size Standard_D2as_v4 \
--admin-username "azureuser" \
--generate-ssh-keys \
--public-ip-sku Standard \
--custom-data cloud-init-jenkins.txt


# Cat VM 

az vm list -d -o table --query "[?name=='jenkins-server-vm']"


# Expose porta 8080 servidor Jenkins

az vm open-port \
--resource-group jenkins-get-started-rg \
--name jenkins-server-vm  \
--port 8080 --priority 1010

# Exposo IP Server

az vm show \
--resource-group jenkins-get-started-rg \
--name jenkins-server-vm -d \
--query [publicIps] \
--output tsv

# Acesso SSH commados

- ssh azureuser@<ip_address>
- service jenkins status
- sudo cat /var/lib/jenkins/secrets/initialAdminPassword
