# Security Oauth2, OIDC, JWT, Keycloak , SpringBoot

# Part 1: Keycloak, Jwt 

## Bullet Points :
### in this part we will cover the following topics:

- Download Keycloak 23
- Start Keycloak
- Create an Admin account
- Create a Realm
- Create a client to secure
- Create users
- Create roles
- Assign roles to users
- Using Postman:
    - Test authentication with the password
    - Analyze the contents of both JWT Access Token and Refresh Token
    - Test authentication with the Refresh Token
    - Test authentication with Client ID and Client Secret
    - Change the parameters of Access Token and Refresh Token

### Screenshots :

#### 1. In the following screenshot, i authenticated with the username and password and we got the Access Token and Refresh Token:
![1 getting data of client via passw](https://github.com/Yahya-rabii/JEE/assets/92509001/c2c6c4c8-8f8c-49c9-a247-bfc4013e8150)


#### 2. In the following screenshot, i decoded the Access Token and we can see its content using jwt.io:
![2 decode the token ](https://github.com/Yahya-rabii/JEE/assets/92509001/72e65d37-d1ab-4329-b68b-0673d22080d5)


#### 3. In the following screenshot, i authenticated with the Refresh Token and we got the new Access Token and Refresh Token:

![3 getting data of client via refresh token](https://github.com/Yahya-rabii/JEE/assets/92509001/0833588d-c41a-4d87-8743-e9bdb87119e6)

#### 4. In the following screenshot, i authenticated with the Client ID and Client Secret and we got the Access Token and Refresh Token:
![4 getting data of client via client secret](https://github.com/Yahya-rabii/JEE/assets/92509001/55e29198-fcd1-4227-8208-1075676c5a9a)


#### 5. In the following screenshot, i changed the capabilitie configuration in keycloak and now even with the client username and password we can't get the Access Token and Refresh Token so we need to use the Client secret and Client ID to get the Access Token and Refresh Token:

![5 getting data of client via password failed](https://github.com/Yahya-rabii/JEE/assets/92509001/f7bb39d2-c62a-481f-93eb-e6256e4fa6a5)


# Part 2: SpringBoot, Keycloak, Jwt , Oauth2 


## Bullet Points :

-   Develop and secure a microservices-based application using OAuth 2, OIDC, and Keycloak:
    - Inventory service
    - Frontend Thymeleaf
    - Frontend Angular


### Screenshots :

#### 1. In the following screenshot, i consulted the customer service and i get the list of customers:
![6 list of customers](https://github.com/Yahya-rabii/JEE/assets/92509001/15fd483d-d5ac-4d95-9c70-3c676bcb5287)


#### 2. In the following screenshot, i added the webjar dependency to the pom.xml file so i can use bootstrap and jquery in my project:
![7 list of customers bootstrap](https://github.com/Yahya-rabii/JEE/assets/92509001/2992f3d8-4f74-4dbb-bdcc-dcf0f00274ed)


#### 3. In the following screenshot, i added the template dependency to the pom.xml file so i can use thymeleaf template in my project that contains the navbar and the footer:
![8 list of customers template ](https://github.com/Yahya-rabii/JEE/assets/92509001/114f2190-2679-46fd-8a46-a722109d110a)


#### 4. In the following gif, i activated the security in the customer service and i configured the login via google so each time i try to access the customer service i will be redirected to the login page and i can login with my google account:
![9 auth with google](https://github.com/Yahya-rabii/JEE/assets/92509001/832d9cba-c9b9-4354-97c8-29b97713d654)

#### In the following gif, i Authenticated with keycloak through a thyemeleaf client, the gif shows that when authenticating with an admin account, we can access the customer service and we can see the list of customers, but when we authenticate with a user account, we can't access the customer service and we get an error message:



#### In the following gif, i Authenticated with keycloak through a angular client using our admin account, the gif shows that we can access the inventory service and we can see the list of products