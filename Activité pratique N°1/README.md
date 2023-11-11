# SOAP Web Services

In this readme file, I will provide a report on the following:

1. The creation of a web service.
2. The deployment of the web service.
3. The consultation and analysis of the WSDL in an HTTP browser.
4. The testing of the web service using SoapUI.
5. The creation of a SOAP client that consumes the web service.

## The Creation of the Web Service

In this part, I created a simple Java class named "BanqueService." I then used the appropriate annotations to transform it into a web service, as shown in the picture below:

![1](https://github.com/Yahya-rabii/JEE/assets/92509001/7b5a291a-8c05-4194-b12e-d8700579bdbd)


## The Deployment of the Web Service

To deploy the web service, I created a class named "ServerJWS." Inside it, I created a main method to publish our web service, making it accessible via any device connected locally through the address http://0.0.0.0:9191, as shown in the picture below:

![2](https://github.com/Yahya-rabii/JEE/assets/92509001/71c704e5-dd52-4f2e-a792-f7c048c72c76)


## The Consultation and Analysis of the WSDL in an HTTP Browser

Now that the web service is published, I can consult the WSDL via the browser using the address http://localhost:9191/?WSDL, as shown in the picture below:

![3](https://github.com/Yahya-rabii/JEE/assets/92509001/8108d763-237d-419a-9808-d8ff74c8f6a3)


## The Testing of the Web Service using SoapUI

To test the methods of the published web service, I used SoapUI as my testing tool. In the picture below, I executed two tests, one before adding the @Transient annotation to the date field of the Account Class:

![4](https://github.com/Yahya-rabii/JEE/assets/92509001/81e115c1-588b-4fad-b315-0660ed97725f)


## The Creation of a SOAP Client that Consumes the Web Service

Finally, to consume the web service, I created a Java client that will use the web service methods, as shown in the picture below:
![5](https://github.com/Yahya-rabii/JEE/assets/92509001/2a2e342c-b3f0-425a-bc36-1fe78d6d2f82)

