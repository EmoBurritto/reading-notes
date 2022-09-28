# Readings: APIs

## API Design Best Practices

API's should have:

Platform independence - Any client should be able to call the API, regardless of how the API is implemented internally. This requires using standard protocols, and having a mechanism whereby the client and the web service can agree on the format of the data to exchange.

Service evolution - The web API should be able to evolve and add functionality independently from client applications. As the API evolves, existing client applications should continue to function without modification. All functionality should be discoverable so that client applications can fully use it.

Many web APIs use JSON as the exchange format

matyrity model:

Level 0: Define one URI, and all operations are POST requests to this URI.
Level 1: Create separate URIs for individual resources.
Level 2: Use HTTP methods to define operations on resources.
Level 3: Use hypermedia (HATEOAS, described below).

Level 3 corresponds to a truly RESTful API according to Fielding's definition. In practice, many published web APIs fall somewhere around level 2.

REST APIs are driven by hypermedia links that are contained in the representation

Avoid requiring resource URIs more complex than collection/item/collection.

(reference: https://learn.microsoft.com/en-us/azure/architecture/best-practices/api-design)
## Questions 

1. What does REST stand for?

Representational State Transfer

2. REST APIs are designed around a ____.

resources, which are any kind of object, data, or service that can be accessed by the client

3. What is an identifier of a resource? Give an example.

 a URI that uniquely identifies that resource; https://adventure-works.com/orders/1

4. What are the most common HTTP verbs?

 GET, POST, PUT, PATCH, and DELETE

5. What should the URIs be based on?

URIs should be based on nouns (the resource) and not verbs (the operations on the resource)

6. Give an example of a good URI.

https://adventure-works.com/orders // Good

7. What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?

web APIs that expose a large number of small resources; bad

8. What status code does a successful GET request return?

HTTP status code 200 (OK)

9. What status code does an unsuccessful GET request return?

404 (Not Found)

10. What status code does a successful POST request return?

HTTP status code 201 (Created)

11. What status code does a successful DELETE request return?

HTTP status code 204 (No Content)

## Things I want to Know more about 
- are there other status code we should memorize or be familar with?
- 22 years is a long time since API's have been created for technology, is there a next big thing in development?