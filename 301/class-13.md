# Readings: More CRUD

## CRUD Basics

CRUD is an acronym that stands for Create, Read, Update and Delete

You can create something new, read or view the newly created data, edit or update the data and finally the option to delete it.

When working with web services, CRUD corresponds to the to HTTP methods, which communications to a web server how you want to interact with a website.

Create
The route for this POST request — /appointments/new

Read
The route for this GET request — /appointments.

Update
The route for this PUT request — /appointments/:id.

Delete
The route for the DELETE request — /appointments/:id

(reference: https://medium.com/geekculture/crud-operations-explained-2a44096e9c88)
## Questions 

1. Which HTTP method would you use to update a record through an API?

PUT

2. Which REST methods require an ID parameter?

PUT
## Speed Coding: Building a CRUD API 


(reference: https://www.youtube.com/watch?v=EzNcBhSv1Wo)
## Questions

1. What’s the relationship between REST and CRUD?

 CRUD is a way of manipulating information, describing the function of an application. 
 REST is controlling data through HTTP commands.

2. If you had to describe the process of creating a RESTful API in 5 steps, what would they be?

1. Identify the resources – Object Modeling
- identifying the objects that will be presented as resources
2. Create Model URIs
- create endpoints for APIs
3. Determine Resource Representations
- refactor to be JSON data
4. Assigning HTTP Methods
-decide all the applications’ possible operations and map those operations to the resource URIs
5. More Actions
-  Logging, Security, Discovery etc.
