#  Express

## 1. What’s the difference between PUT and PATCH?
- PUT is a method of modifying resource where the client sends data that updates the entire resource. It is used to set an entity’s information completely.

- Unlike PUT, PATCH applies a partial update to the resource.
This means that you are only required to send the data that you want to update, and it won’t affect or change anything else. So if you want to update the first name on a database, you will only be required to send the first parameter; the first name.

## 2. Provide links to 3 services or tools that allow you to “mock” an API for development like json-server

[1. WireMock](http://wiremock.org/)

[2. Postman Mock Server](https://learning.postman.com/docs/designing-and-developing-your-api/mocking-data/setting-up-mock/)

[3. Stoplight](https://stoplight.io/mocking/)

## 3. Compare and contrast Swagger and APIDoc.js 1 Which HTTP status codes should be sent with each type of (un)successful API call?

  responses:
        '200':
          description: OK

        '400':
          description: Bad request. User ID must be an integer and larger than 0.

        '401':
          description: Authorization information is missing or invalid.

        '404':
          description: A user with the specified ID was not found.

        '5XX':
          description: Unexpected error.


## 4. Compare and contrast SOAP and ReST

The difference is:

1. SOAP is a XML-based message protocol, while REST is an architectural style

2. SOAP uses WSDL for communication between consumer and provider, whereas REST just uses XML or JSON to send and receive data

3. SOAP invokes services by calling RPC method, REST just simply calls services via URL path

4. SOAP doesn't return human readable result, whilst REST result is readable with is just plain XML or JSON

5. SOAP is not just over HTTP, it also uses other protocols such as SMTP, FTP, etc, REST is over only HTTP
