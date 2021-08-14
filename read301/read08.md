## Things I want to know more about

# APIs

**API Design Best Practices**

1. What does REST stand for?

  - REST stands for Representational State Transfer. (It is sometimes spelled "ReST".)
    It relies on a stateless, client-server, cacheable communications protocol -- and 
    in virtually all cases, the HTTP protocol is used.

2. REST APIs are designed around a resources.


3. What is an identifer of a resource? Give an example.

  - genes, organisms, tools, and reagents (such as antibodies).


4. What are the most common HTTP verbs?

  - Are POST, GET, PUT, PATCH, and DELETE.


5. What should the URIs be based on?

  - Resource Description Framework.

6. Give an example of a good URI:

  - example.com/articles/good-uri-design.


7. What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?

  -  is one that requires consumer to make tremendous (subjective matter) amount 
     of distinct API calls to get needed information about a resource. George Reese
     has defined chatty API as any API that requires consumer to do more than a single 
     call to perform a single, common operation. its poor quality.


8. What status code does a successful GET request return?

  - 2xx Successful: This means the server successfully processed the request, but
   is not returning any content.

9. What status code does an unsuccessful GET request return?

  - 412:“Precondition Failed.” Your browser included certain conditions in its request
    headers, and the server did not meet those specifications.

10. What status code does a successful POST request return?

  - The origin server MUST create the resource before returning the 201 status code.


11. What status code does a successful DELETE request return?

  - A 202 ( Accepted ) status code if the action will likely succeed but has not yet been enacted.

  