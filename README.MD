# IoT in the Cloud with node-red

In this workshop, you will get to work with the IoT possibilities of the AWS platform. Since working with a hardware device brings several problems with it, we will be using node-red to emulate the IoT client since it supports the MQTT protocol and works out-of-the-box with the certificates created by AWS.

A visualisation has been added to node-red, which will allow you to have a row of "LED" lights and to play sounds and which can be controlled by using a data source in node-red. The visualisation itself can be found on the `/dash` path of the domain where node-red is running.

More information about node-red and how to use it will be demo-ed before the workshop. 

To control your device (i.e., emulating the controlling computer) you can also use node-red. However, you are also allowed to execute the control code on your computer and/or use the AWS IoT testing web application to send or receive data on MQTT topics.

## List of use cases

Below you will find a list of possible use cases. However, you are allowed to be creative in your implementation of the use cases. You may also 

* Incoming blink: Blink a light everytime an mqtt message arrives
* Use the IoT shadow to create the Knightrider pattern with the lights
* Create a topic on which to request a quote by sending a message. Use a lambda to respond to the message with a random quote.
* Store messages of a given topic in DynamoDB
* use the IoT shadow to send the link of an mp3 file stored in S3 to play

## Useful links

* [IoT Device Shadows AWS Documentation](https://docs.aws.amazon.com/iot/latest/developerguide/iot-device-shadows.html)
* [AWS DynamoDB Documentation](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Introduction.html)
* [AWS Lambda Documentation](https://docs.aws.amazon.com/lambda/latest/dg/welcome.html)