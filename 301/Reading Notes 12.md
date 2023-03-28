# Status Codes based on REST Methods

## Status
In your own words, describe what each group of status code represents:

100’s = s'okay
200’s = Good connection. You did it. God bless.
300’s = redirection
400’s = client error
500’s = server error

1. What is a status code 202? 
- The HyperText Transfer Protocol (HTTP) 202 Accepted response status code indicates that the request has been accepted for processing, but the processing has not been completed; in fact, processing may not have started yet.

2. What is a status code 308?
- The HyperText Transfer Protocol (HTTP) 308 Permanent Redirect redirect status response code indicates that the resource requested has been definitively moved to the URL given by the Location headers.
3. What code would you use if an update didn’t return data to a client?
- 204 No Content
4. What code would you use if a resource used to exist but no longer does?
- HTTP 409
5. What is the ‘Forbidden’ status code?
- HTTP 403

## Build API node.js, express and mongodb

1. Why do we need to pull our MongoDB database string out of our server and put it into our .env?
- To give the server a pointer to our MongoDB database
2. What is middleware?
- Middleware is software that lies between an operating system and the applications running on it
3. What does app.use(express.json()) do?
- parse the incoming requests with JSON payloads 
4. What does the /:id mean in a route?
- /:id is the path that gets you to this function.
5. What is the difference between PUT and PATCH?
- PUT is a technique of altering resources when the client transmits data that revamps the whole resource. PATCH is a technique for transforming the resources when the client transmits partial data that will be updated without changing the whole data.
6. How do you make a default value in a schema?
- const schema = new Schema({
  name: String,
  role: { type: String, default: 'guitarist' }
  });
7. What does a 500 error status code mean?
- The HyperText Transfer Protocol (HTTP) 500 Internal Server Error server error response code indicates that the server encountered an unexpected condition that prevented it from fulfilling the request.
8. What is the difference between a status 200 and a status 201?
- 200: “Everything is OK.” This is the code that is delivered when a web page or resource acts exactly the way it's expected to. 201: “Created.” The server has fulfilled the browser's request, and as a result, has created a new resource

## Things I want to know more about