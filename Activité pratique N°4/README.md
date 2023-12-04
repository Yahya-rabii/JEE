# Spring-Boot/Angular full stack ecom web app 


## Description

This is a full stack ecom web app built with Spring Boot and Angular. It is a simple ecom web app that allows users to see products and their orders.
The backend is built using Spring Boot and the frontend is built using Angular. 
for the database, I used h2 database which is an in-memory database.

## How to run the app

### Backend

To run the backend, you need to have Java 8 or higher installed on your machine.

1. Clone the repo
2. create a config folder locally and add a file called `application.properties` and add the following properties to it:
```properties
spring.h2.console.enabled=true
management.endpoints.web.exposure.include=*
```
2. Run consul discovery service after downloading it from https://developer.hashicorp.com/consul/install
use the following command to run consul:
```bash
    cd 'where you downloaded consul'
    ./consul.exe agent -server -bootstrap-expect=1 -data-dir="C:\Users\yahya\Desktop\consul\Data" -ui -bind='your ip address'
```


3. Open the project backend folder in your IDE and run each microservice separately 
4. Run the backend application classes
5. Go to http://localhost:8082/h2-console to visualize the running microservices

### Frontend

#### To run the frontend, you need to have node.js and angular cli installed on your machine
1. Open the project frontend folder in your IDE and run the frontend application 
2. Download the node modules by running the following command:
```bash
    npm install
```

3. run the frontend app by running the following command:
```bash
    ng serve
```

4. test the app by going to http://localhost:4200




## Screenshots and description

### consule discovery service (first lunch)

#### in the first lunch, the consul discovery service will contain only the consul service itself and the config service as shown in the following screenshot:

![1cosullunched](https://github.com/Yahya-rabii/JEE/assets/92509001/cbae6db5-e901-47f9-9428-e02767a37ff4)


### consulting the CUSTOMER-SERVICE microservice's default properties

#### the following screenshot shows the default properties of the CUSTOMER-SERVICE microservice via the gateway service:

![2 consulting customarserv default](https://github.com/Yahya-rabii/JEE/assets/92509001/d2bebab4-d981-46c4-a760-6511f9de04db)



### consulting the CUSTOMER-SERVICE microservice's dev properties

#### the following screenshot shows the dev properties of the CUSTOMER-SERVICE microservice via the gateway service:


![3 consulting customarserv dev](https://github.com/Yahya-rabii/JEE/assets/92509001/d7dea890-397c-496a-a84c-c832f039878c)


### consulting the CUSTOMER-SERVICE microservice's prod properties

#### the following screenshot shows the prod properties of the CUSTOMER-SERVICE microservice via the gateway service:


![4 consulting customarserv prod](https://github.com/Yahya-rabii/JEE/assets/92509001/e9f12f64-e3ab-4580-82b8-22482eb68b0b)


### consul discovery service (second lunch)

#### in the second lunch, the consul discovery service will contain the customer-service microservice as shown in the following screenshot:


![5cosul ](https://github.com/Yahya-rabii/JEE/assets/92509001/47403329-0946-4e18-93c3-08a1bada95b5)



### consul discovery service (third lunch)

#### in the third lunch, the consul discovery service will contain the gateway-service microservice as shown in the following screenshot:




![7 cosul ](https://github.com/Yahya-rabii/JEE/assets/92509001/ca165dbe-f609-4fe8-bc2f-6339e2f31fe5)




### consulting the CUSTOMER-SERVICE microservice's via the gateway service

#### the following screenshot shows the list of customers in the CUSTOMER-SERVICE microservice via the gateway service:


![7consulting the service of cust via gatway ](https://github.com/Yahya-rabii/JEE/assets/92509001/c45d278c-cb70-4fc7-b169-86c229e90dda)


### consul discovery service (fourth lunch)

#### in the fourth lunch, the consul discovery service will contain the inventory-service microservice as shown in the following screenshot:



![8 consul inventoryser](https://github.com/Yahya-rabii/JEE/assets/92509001/07d37438-2578-4b20-9933-9bd830e8851a)


### consulting the list of products in the INVENTORY-SERVICE microservice via the gateway service


#### the following screenshot shows the list of products in the INVENTORY-SERVICE microservice via the gateway service:

![10 consulting the service of inventoroies via gateway ](https://github.com/Yahya-rabii/JEE/assets/92509001/7042dc23-85a9-434d-a6d4-f6f9dbc91d28)



### consulting the list of products and customers using a projection 


#### the following screenshot shows the list of products and the list of customers in both the INVENTORY-SERVICE and the CUSTOMER-SERVICE microservices using a projection via the gateway service:



![11 Projection](https://github.com/Yahya-rabii/JEE/assets/92509001/ec890bd9-5f18-4bd8-a07d-5240aaea1a10)


### consulting the list of orders in the ORDER-SERVICE microservice via the gateway service


#### the following screenshot shows the list of orders in the ORDER-SERVICE microservice via the gateway service:



![12 order service orders](https://github.com/Yahya-rabii/JEE/assets/92509001/a0692dda-95e8-40bb-a7f0-f2ca9dcfa3ba)



### consulting the items list of the order with id 5 in the ORDER-SERVICE microservice via the gateway service


#### the following screenshot shows the items list of the order with id 5 in the ORDER-SERVICE microservice via the gateway service:


![13 order service product Items ](https://github.com/Yahya-rabii/JEE/assets/92509001/03accf98-b544-408c-ad2f-b52eb03ce914)




### consulting the full order of the first order in the ORDER-SERVICE microservice via the gateway service


#### the following screenshot shows the full order of the first order in the ORDER-SERVICE microservice via the gateway service:



![14 full order](https://github.com/Yahya-rabii/JEE/assets/92509001/3f26aff1-ed76-4e3c-83ee-a0017d9c23c1)



### consul discovery service (final state)


#### the following screenshot shows the final state of the consul discovery service after running all the microservices:



![15 cosul ](https://github.com/Yahya-rabii/JEE/assets/92509001/104c61ef-d33f-406a-9eb5-7304a39f1e44)




### getting the properties via consul discovery service and vault 


#### the following screenshot shows how to get the properties stored in vault and consul discovery service via a spring boot microservice:


![16 getting data from consul config and vault ](https://github.com/Yahya-rabii/JEE/assets/92509001/621862dc-f4f5-42c2-a630-ac6035728511)


## video demo of the app 


#### the following video shows a demo of the app:

[![Watch the video](https://i9.ytimg.com/vi/TjJLwVZ7ti8/mqdefault.jpg?v=656de2e7&sqp=COjEt6sG&rs=AOn4CLDrScmJP7DRLQ74hrYsAxDsVYtn6w)](https://youtu.be/TjJLwVZ7ti8)



## Author

[![yahya rabii](https://yahya.rabii.me/images/Yahya%20Rabii.png)](https://yahya.rabii.me/)













