# kafka producer and consumer and functional programming with spring boot

this project is a spring boot application that uses kafka to send and receive messages, and also uses functional programming with spring boot.

## screenshots

the first screenshot shows 2 windows, the first one showws the publisher in the web browser, and the second one shows the consumer in the terminal.





the second screenshot shows the terminal of the consumer, where we can see our custom message identified in the pageEventConsumer Bean in our service.




the third screenshot shows the producer in the terminal and the terminal of the consumer, where we can see our custom message



the fourth screenshot shows the Function<PageEvent, PageEvent> pageEventPageEventFunction function that is used to transform the message received by the consumer, and the terminal of the consumer, where we can see json message transformed by the function.


the fifth screenshot shows the Function<PageEvent, PageEvent> kstreamPageEventPageEventFunction function that is used to transform the message received by the consumer, and the terminal of the consumer, where we can see json message transformed by the function.


the last screenshot shows the analytics in the terminal of the consumer, where we can see the number of events per page. and the analytics graph in the web browser that shows the number of events per page in real time using smoothie.js library.



## Author

[![yahya rabii](https://yahya.rabii.me/images/Yahya%20Rabii.png)](https://yahya.rabii.me/)


