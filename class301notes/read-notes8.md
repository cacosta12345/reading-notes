# Reading Notes Class 8

# API Design Best Practices

1. What does REST stand for?

    * Representational State Transfer (REST)

2. REST APIs are designed around a ____.

    * resource

3. What is an identifier of a resource? Give an example.

    * a URI that uniquely identifies that resource

    * ex. https://adventure-works.com/orders/1

4. What are the most common HTTP verbs?

    * GET, POST,  PUT, PATCH, DELETE

5. What should the URIs be based on?

    * URIs should be based on nouns (the resource) and not verbs (the operations on the resource).

6. Give an example of a good URI.

    * https://adventure-works.com/orders // Good

    * https://adventure-works.com/create-order // Avoid

7. What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?

    * Another factor is that all web requests impose a load on the web server. The more requests, the bigger the load. Therefore, try to avoid "chatty" web APIs that expose a large number of small resources. Such an API may require a client application to send multiple requests to find all of the data that it requires.

8. What status code does a successful GET request return?

    * 200 OK

9. What status code does an unsuccessful GET request return?

    * 204

10. What status code does a successful POST request return?

    * 201 Created

11. What status code does a successful DELETE request return?

    * 204 No Content