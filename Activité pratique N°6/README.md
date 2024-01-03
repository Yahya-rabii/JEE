# kafka producer and consumer and functional programming with spring boot

this project is a spring boot application that uses kafka to send and receive messages, and also uses functional programming with spring boot.

## screenshots

the first screenshot shows 2 windows, the first one showws the publisher in the web browser, and the second one shows the consumer in the terminal.


![1 publish via console-consumer ](https://github.com/Yahya-rabii/JEE/assets/92509001/3d9df9da-1753-4815-895b-2a9f74cd50fc)



the second screenshot shows the terminal of the consumer, where we can see our custom message identified in the pageEventConsumer Bean in our service.


![2 service ](https://github.com/Yahya-rabii/JEE/assets/92509001/1df4b00e-a513-4414-85c2-55e761a1c1ca)


the third screenshot shows the producer in the terminal and the terminal of the consumer, where we can see our custom message


![3 prod to client aka consumer](https://github.com/Yahya-rabii/JEE/assets/92509001/6f06186b-e98b-421b-a074-e8e32a6720af)

the fourth screenshot shows the Function<PageEvent, PageEvent> pageEventPageEventFunction function that is used to transform the message received by the consumer, and the terminal of the consumer, where we can see json message transformed by the function.
![4 supplier](https://github.com/Yahya-rabii/JEE/assets/92509001/b8dab1af-41f5-4870-8dfd-9a39bdc5065f)


the fifth screenshot shows the Function<PageEvent, PageEvent> kstreamPageEventPageEventFunction function that is used to transform the message received by the consumer, and the terminal of the consumer, where we can see json message transformed by the function.

![5 Function png](https://github.com/Yahya-rabii/JEE/assets/92509001/34bc20ef-5121-466f-8d8d-e190ef0bfe06)

the last screenshot shows the analytics in the terminal of the consumer, where we can see the number of events per page. and the analytics graph in the web browser that shows the number of events per page in real time using smoothie.js library.

![7 graphs](https://github.com/Yahya-rabii/JEE/assets/92509001/c1805ebf-b6a8-4c0c-916c-4262c642f295)


## Author

[![yahya rabii](https://yahya.rabii.me/images/Yahya%20Rabii.png)](https://yahya.rabii.me/)


