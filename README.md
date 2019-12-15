# invent

# Create PV for mysql:



# Install mysql via helm chart:
helm install mysql stable/mysql --values helm/helm-configs/mysql-values.yaml


# Access mysql:
# Ubunutu pod - 
kubectl run -i --tty ubuntu --image=ubuntu:16.04 --restart=Never -- bash -i
apt-get update && apt-get install mysql-client -y
mysql -h mysql -u invent -p invent
use invent


# Mysql client pod - 

# Commands: