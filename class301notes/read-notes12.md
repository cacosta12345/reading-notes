# Reading Notes Class 12

## Status Codes On REST Methods

1. In your own words, describe what each group of status code represents:

100’s = informational, tell the client header has been recieved and will try getting

200’s = Success! The request went through

300’s = Tell the client the resource they want isn't available

400’s = Client error. Could be bad payload, miss-spelling, bad url. Something on the client's side

500’s = Server error. Could be a problem at server.

2. What is a status code 202?

    * Often used for asynchronous processing. This code tells the client that the request was valid, but its processing will finish sometime in the future. The response body should include an URL to the finished resource with some information about when it will be available, or an URL to some monitoring endpoint that tells the client when the resource is available.

3. What is a status code 308?

    * Like the 202 code but using a Location header field in response to informing the client about the location of the created resource or an endpoint that lets the client check for the status of the creation process. Some clients follow the status codes of the Redirect-class automatically. This code is usually only used for POST requests.

4. What code would you use if an update didn’t return data to a client?

    * 204

5. What code would you use if a resource used to exist but no longer does?

    * 308 Permanent redirect

6. What is the ‘Forbidden’ status code?

    * 403 Forbidden The client has authorized or doesn’t need to authorize itself, but still has no permissions to access the resource.

## Build A REST API With Node.js, Express, & MongoDB - Quick

1. Why do we need to pull our MongoDB database string out of our server and put it into our .env?

    * .env contains info you don't want public. We need the mongodb string to connect to the database

2. What is middleware?

    * Middleware refers to software that acts as an intermediary between different applications, systems, or components to facilitate communication and data exchange. 

3. What does app.use(express.json()) do?

    * In the context of a Node.js application using the Express.js framework, the app.use(express.json()) statement is middleware that is used to parse incoming requests with JSON payloads

4. What does the /:id mean in a route?

    * :id is a placeholder for a dynamic value that can be different for each request.

5. What is the difference between PUT and PATCH?

    * Put updates a resource be replacing whole thing

    * Patch is a partial update. Updates a piece of existing resource

6. How do you make a default value in a schema?

    * const userSchema = new mongoose.Schema({})

7. What does a 500 error status code mean?

    * Server side error or generic error message

8. What is the difference between a status 200 and a status 201?

    * 200 Successful GET

    * 201 Successful POST