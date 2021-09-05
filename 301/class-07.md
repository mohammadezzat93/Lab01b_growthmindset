# REST

![Rest](https://cdn-media-1.freecodecamp.org/images/1*gqHgCNubMncv7EwWNdArGQ.png)

## How I explained REST to my brother

### Who is Roy Fielding?
- Some guy. He's smart.
- He helped write the first web servers, that sent documents across the internet… and then he did a ton of research explaining why the web works the way it does. His name is on the specification for the protocol that is used to get pages from servers to your browser.

### Why don’t the techniques that we use today work well when we need to be able to talk to all of the machines in the world?
-Because they weren't designed to be used like that. When Fielding and his colleagues started building the web, being able to talk to any machine anywhere in the world was a primary concern. But most of the techniques developers later used to get computers to talk to each other didn't have those requirements. You just needed to talk to a small group of machines.

### What is the HTTP protocol that Fielding and his friends created?
- That first part tells the browser what protocol to use. That stuff you type in there is one of the most important breakthroughs in the history of computing.

- The Hypertext Transfer Protocol (HTTP) is designed to enable communications between clients and servers.

- HTTP works as a request-response protocol between a client and server.

### What does a GET do?
-GET is used to request data from a specified resource.

### What does a POST do?
-POST is used to send data to a server to create/update a resource.

- The data sent to the server with POST is stored in the request body of the HTTP request

### What does PUT do?
- PUT is used to send data to a server to create/update a resource.

- **The difference** between POST and PUT is that PUT requests are idempotent. That is, calling the same PUT request multiple times will always produce the same result. In contrast, calling a POST request repeatedly have side effects of creating the same resource multiple times.

### What does PATCH do?
- This includes fixing security vulnerabilities and other bugs, with such patches usually being called bugfixes or bug fixes

# API Keys
## Geocoding API
Did you get your API key?
- Yes
## Weather Bit API
Did you get your API key?
- Yes
## Yelp API Docs
Did you get your API key?
- Yes
## The Movie DB API Docs
Did you get your API key?
- Yes

![APIS](https://miro.medium.com/max/1124/1*YLFt-xYVwkrDx-S4CnsoEQ.png
)