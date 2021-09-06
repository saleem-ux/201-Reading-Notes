# AWS: API, Dynamo and Lambda

![](https://miro.medium.com/max/650/1*XuR8U6TOa5ar88lf2IbNNQ.png)

## Review, Research, and Discussion

**What are serverless functions?**

- its a code that executed directly in cloud without thinking of maintaining servers.

![](https://stackify.com/wp-content/uploads/2017/05/what-is-function-as-a-service-serverless-architectures-are-here-11196.png)

**If you were to create a system that emulated Lambda functions, how would you do it?**

- only you have to write your code inside handler function for Lambda either online or locally and then upload the code. 
- after that you have to trigger this Lambda function with other services to execute it.

**Describe how a CDN works**

- it is a group of servers that connected together, but each one of them in different location.
- when a user hit a request, then the nearest server to the user's region will response to it.

![](https://www.globaldots.com/hs-fs/hubfs/cdne.png?width=590&name=cdne.png)

# Document the following Vocabulary Terms

**Serverless Functions** it's a code that executed directly in cloud without thinking of maintaining servers.

**Cloud Storage** a service that allows you to save your static data online and use them when ever you want.

**CDN** Content delivery network, it is a group of servers that connected together, but each one of them in different location. when a user hit a request, then the nearest server to the user's region will response to it.

# Preparation Materials

# AWS API Gateway Overview

- Amazon API Gateway is a managed service that allows developers to define the HTTP endpoints of a REST API or a WebSocket API and connect those endpoints with the corresponding backend business logic. It also handles authentication, access control, monitoring, and tracing of API requests.

- API Gateway mostly used with serverless functions to replace API servers.

- it run Lambda functions to generate HTTP API responses.

- it can publish SNS notifications when an HTTP API endpoint is accessed.

- API Gateway provide authentication and authorization for your HTTP APIs.

### advantages of using API Gateway AWS :

  - response to HTTP API requests.
  - response to WebSocket requests.
  - using AWS cognito that will check the authorization for your app, then no need to use your own auth.
  - using cloudWatch, X-Ray and another logging AWS services to simplify the debugging of your API requests.

![](https://miro.medium.com/max/700/0*rR1grG94IwM1JGI8)


### dissadvantages of using API Gateway :

  - in some cases, response time will be slow.
  - Payload size : 10 MB
  - Integration timeouts : from 50 ms to 29 sec
  - Regional APIs : 600 regional API

- but maybe you can enhance some of these limits if contacted the AWS support.


# AWS API Gateway

- Amazon API Gateway is a fully managed service that makes it easy for developers to create, publish, maintain, monitor, and secure APIs at any scale.


# AWS DynamoDB Guide

- DynamoDB is a hosted NoSQL database offered by Amazon Web Services (AWS). 

- DynamoDB good for:

  - Applications with large amounts of data and strict latency requirements (up to 100 TBs)
  - Serverless applications using AWS Lambda
  - Data sets with simple, known access patterns


# AWS DynamoDB

- Amazon DynamoDB is a key-value and document database that delivers single-digit millisecond performance at any scale. It's a fully managed, multi-region, multi-active, durable database with built-in security, backup and restore, and in-memory caching for internet-scale applications. DynamoDB can handle more than 10 trillion requests per day and can support peaks of more than 20 million requests per second.

- very fast response (in milli-seconds).
- it can handle a huge amount of requests togother.


# Dynamoose

- Dynamoose is a modeling tool for Amazon's DynamoDB. Dynamoose is heavily inspired by Mongoose, which means if you are coming from Mongoose the syntax will be very familiar.

- it is a package that we have to install on our terminals to control the AWS DynamoDB service to use NoSQl database.

- installation command :
 
```
npm install dynamoose
```


```
## External resources :
```
- [https://www.docker.com/resources/what-container](https://www.docker.com/resources/what-container)
- [https://www.paessler.com/it-explained/bandwidth](https://www.paessler.com/it-explained/bandwidth)
- [https://expedient.com/knowledgebase/blog/2015-05-01-how-the-cost-of-cloud-computing-is-calculated/](https://expedient.com/knowledgebase/blog/2015-05-01-how-the-cost-of-cloud-computing-is-calculated/)

* [stackoverflow](https://stackoverflow.com/questions/7042340/error-cant-set-headers-after-they-are-sent-to-the-client?rq=1)


* [https://kumargaurav1247.medium.com/aws-sns-simple-notification-service-1972262b8564](https://kumargaurav1247.medium.com/aws-sns-simple-notification-service-1972262b8564)


* [AWS](https://aws.amazon.com/ec2/?ec2-whats-new.sort-by=item.additionalFields.postDateTime&ec2-whats-new.sort-order=desc)


* [EC2 For Humans](https://www.youtube.com/watch?v=lZMkgOMYYIg)


* [Elastic Beanstalk](https://www.youtube.com/watch?v=SrwxAScdyT0)