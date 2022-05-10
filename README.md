# Rancher Hadoop Hive - Docker
Rancher Hadoop Hive - Docker

## Kompose (kurbenets or openshift)
Converting docker-compose to kurbenets kompose: https://kompose.io/

## Rancher

1. Install rancher: ``` $ brew install --cask rancher ```
1. (if no brew) Install rancher desktop: https://rancherdesktop.io/
1. Open Rancher Desktop > Kurbenets Settings : select "dockerd"
1. All docker images gona be available on "rancher images"


```shell
    # Creating and starting a service without environment variables and selecting a stack
    # If no stack is provided, the stack name will be the folder name that the command is running from
    # If the stack does not exist in Rancher, it will be created
    $ rancher-compose --url URL_of_Rancher --access-key <username_of_environment_api_key> --secret-key <password_of_environment_api_key> -p stack1 up

    # Creating and starting a service with environment variables already set
    $ rancher-compose -p stack1 up

    # To change the scale of an existing service
    $ rancher-compose -p stack1 scale service1=3
```

## Hadoop Docker

## Hive Docker
