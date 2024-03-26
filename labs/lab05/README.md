# Lab 05 - Deploy Inventory Microservice

In this hack-a-thon, you will use Docker images provided for you to create a set of microservices that enable management of a toyshop's inventory.

![](arch.png)

## Inventory operations

### Get current inventoy for a toy

GET against http://localhost:5100/inventory/{productNumber}. Allows view of inventory to confirm automatically initialized to 50 on creation of a new toy.

## Deploy to Kubernetes

Using `gamuttechsvcsllc/inventory-svc:1.0` and the `mysql` image, create manifests to deploy the inventory microservice to k8s along with a database. Use Services to enable access to the defined API routes and access to the MySQL database from the services. Use ConfigMaps and Secrets where appropriate for storage and provision of configuration detail. Also, leverage PersistentVolumeClaims where relevant to maintain required data across any Pod replacements.

For `inventory` service, config currently looks like this:

MYSQL_DATABASE = inventory_db  
MYSQL_PASSWORD = pass
MYSQL_USERNAME = root
MYSQL_SERVICE_HOST = localhost
