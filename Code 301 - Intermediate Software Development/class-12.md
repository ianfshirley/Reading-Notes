## CRUD

### Status Codes Based On REST Methods

1. In your own words, describe what each group of status code represents:

- 100’s = Informational - header part of request received
- 200’s = Success - request accepted
- 300’s = Redirection - requested resource unavailable, new req to new location
- 400’s = Client Error - invalid requests
- 500’s = Server Error - Server has problems or is overwhelmed

2. What is a status code 202?
- Accecpted, often used for async processing. Request was valid but the processing will happen later
3. What is a status code 308?
- Permanent redirect: tells client to use another URL to access the resource instead of current URL
4. What code would you use if an update didn’t return data to a client?
- 204 No Content
5. What code would you use if a resource used to exist but no longer does?
- 410 Gone
6. What is the ‘Forbidden’ status code?
- 403

### Build A REST API With Node.js, Express, & MongoDB - Quick

1. Why do we need to pull our MongoDB database string out of our server and put it into our .env?
- To protect our sensitive information
2. What is middleware?
- Code that runs when the server gets a request, before it gets passed to your routes
3. What does app.use(express.json()) do?
- It sets up the server to accept JSON as a body
4. What does the /:id mean in a route?
- The id is a parameter for the request, which refers to a single document in the DB
5. What is the difference between PUT and PATCH?
- Patch updates only what the user passed in, rather than the entire item/document
6. 7. How do you make a default value in a schema?
- Use the 'default' property. Inside of a key object, along with type, required etc., write 'default:' and whatever you want the default property to be.
8. What does a 500 error status code mean?
- Server error
9. What is the difference between a status 200 and a status 201?
- 200 is generic success status, 201 means success, resource created


### Sources

[Status Codes Based On REST Methods](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)<br>
[Build A REST API With Node.js, Express, & MongoDB - Quick](https://www.youtube.com/watch?v=fgTGADljAeg)<br>