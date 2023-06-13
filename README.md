# Azure-Jenkins-Sonar-LABS Devops -- CLOUD AZURE

- Setup resource Group basico.

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


# Exposo porta 8080 servidor Jenkins

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
