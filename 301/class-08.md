# APIs

## API Design Best Practices

### What does REST stand for?
- A primary advantage of REST over HTTP is that it uses open standards, and does not bind the implementation of the API or the client applications to any specific implementation. For example, a REST web service could be written in ASP.NET, and client applications can use any language or toolset that can generate HTTP requests and parse HTTP responses.

### REST APIs are designed around a ____.
- resources

### What is an identifer of a resource? Give an example.
- which are any kind of object, data, or service that can be accessed by the client.
- A resource has an identifier, which is a URI that uniquely identifies that resource. For example, the URI for a particular customer order might be:

      https://adventure-works.com/orders/1

### What are the most common HTTP verbs?
- GET, POST, PUT, PATCH, and DELETE.

### What should the URIs be based on?
- A resource has an identifier, which is a URI that uniquely identifies that resource

### Give an example of a good URI.
- https://adventure-works.com/orders // Good

### What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?
- try to avoid "chatty" web APIs that expose a large number of small resources. Such an API may require a client application to send multiple requests to find all of the data that it requires. Instead, you might want to denormalize the data and combine related information into bigger resources that can be retrieved with a single request.
- it is bad
### What status code does a successful GET request return?
- A successful GET method typically returns HTTP status code 200 (OK)

### What status code does an unsuccessful GET request return?
- If the resource cannot be found, the method should return 404 (Not Found).

### What status code does a successful POST request return?
- it returns HTTP status code 201 (Created).

### What status code does a successful DELETE request return?
- If the delete operation is successful, the web server should respond with HTTP status code 204 (No Content)
