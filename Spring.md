## Deploy Spring microservices to Azure
1. Create a new Azure Spring Cloud cluster
    ```bash
    az extension add -n spring-cloud -y

    RESOURCE_GROUP_NAME=spring-cloud-workshop
    SPRING_CLOUD_NAME=azure-spring-cloud-workshop

    az group create \
      -g "$RESOURCE_GROUP_NAME" \
      -l eastus

    az spring-cloud create \
      -g "$RESOURCE_GROUP_NAME" \
      -n "$SPRING_CLOUD_NAME" \
      --sku standard \
      --enable-java-agent

    az configure --defaults group=${RESOURCE_GROUP_NAME}
    az configure --defaults spring-cloud=${SPRING_CLOUD_NAME}
    ```
1. Configure a Spring Cloud Config Server
    - hook up to your git repo
1. Build and deploy a Spring Boot microservice
1. Create a Spring Cloud Gateway to access your microservice
1. Use Spring Cloud Service Registry to discover your microservice
1. Configure distributed tracing to debug a microservices architecture

