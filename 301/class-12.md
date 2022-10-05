# Readings: CRUD

## Status Codes Based On REST Methods

A status code is a number higher than 100 and smaller than 600 that is part of a HTTP response. 

The first digit defines the class of the status.

(reference: https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)
## Questions 

1. In your own words, describe what each group of status code represents:

100’s = request received, in que 
200’s = request received, success 
300’s = request received, data no longer valid in this location 
400’s = invalid request, problem with user request 
500’s = invalid request, problem with server 
2. What is a status code 202?

This code tells the client that the request was valid, but its processing will finish sometime in the future.

3. What is a status code 308?

This tells the client to use another URL to access the resource and not use the current URL anymore. 

4. What code would you use if an update didn’t return data to a client?

204 no content 

5. What code would you use if a resource used to exist but no longer does?

307 Temporary Redirect 

6. What is the ‘Forbidden’ status code?

403 Forbidden - The client has authorized or doesn’t need to authorize itself, but still has no permissions to access the resource.

## Build A REST API With Node.js, Express, & MongoDB - Quick -


(reference: https://www.youtube.com/channel/UCFbNIlppjAuEX4znoulh0Cw)
## Questions

1. Why do we need to pull our MongoDB database string out of our server and put it into our .env?

no longer use localhost when deployed 

2. What is middleware?

middleman 

3. What does app.use(express.json()) do?

allows get to be read in JSON to be added in MongoDB

4. What does the /:id mean in a route?

the specific ID in a JSON data table to get right object

5. What is the difference between PUT and PATCH?

PUT is a method of modifying resource where the client sends data that updates the entire resource . 
PATCH is a method of modifying resources where the client sends partial data that is to be updated without modifying the entire data.

6. How do you make a default value in a schema?

If you create a new document without that path set, the default will kick in.

7. What does a 500 error status code mean?

problem with server; 500 Internal Server Error server error response code indicates that the server encountered an unexpected condition that prevented it from fulfilling the request. This error response is a generic "catch-all" response.

8. What is the difference between a status 200 and a status 201?

The 200 status code is by far the most common returned. It means, simply, that the request was received and understood and is being processed. 
A 201 status code indicates that a request was successful and as a result, a resource has been created (for example a new page).

