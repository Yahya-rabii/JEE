# Angular - Json Server web application

this is a simple web application that uses Angular and Json Server to create a simple web application that can be used to create, read, update and delete data from a json file.


## Installation

clone the repository and run the following commands:

```bash
npm install
```

make sure you have json-server installed globally, if not run the following command:

```bash
npm install -g json-server
```

## Usage

1- make sure you have data/db.json file in the root directory of the project, if not create one and add the necessary data.

2- to run the application, run first the json-server using the following command:

```bash
json-server --watch data/db.json --port 8080
```

3- then run the angular application using the following command:

```bash
ng serve
```

4- open your browser and go to http://localhost:4200/ to see the application running.


## screenshots

the first screenshot shows the login page, where the user can login using his username and password.




the second screenshot shows the home page, where the user can see the navigation bar and the logout button next to its username.



the third screenshot shows the products page, where the user can see the list of products and search for a specific product using the search bar.



the fourth screenshot shows the add product page, where the user can't add a product unless he is an admin.



the last screenshot shows that for an admin user, the add product component is available and he can add a product to the list of products.




## Author

[![yahya rabii](https://yahya.rabii.me/images/Yahya%20Rabii.png)](https://yahya.rabii.me/)


