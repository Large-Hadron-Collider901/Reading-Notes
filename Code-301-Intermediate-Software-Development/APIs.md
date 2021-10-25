# API Design Best Practices

**1. What does REST stand for?**

 [R] [E]presentational [S]tate [T]ransfer 

**2. REST APIs are designed around a ____.**

Resource

**3. What is an identifier of a resource? Give an example.**

An identifier of a resource is a URI (uniform resource identifier) that uniquely identifies a resource. One example of a resource identifier would be a URI that allows us to read account information for a customer with the ID #22354, which would look similar to this => `GET http://www.example.com/customers/22354`

**4. What are the most common HTTP verbs?**

GET, POST, PUT, PATCH and DELETE

**5. What should the URIs be based on?**

URIs should be based on nouns (the resource) rather than verbs.

**6. Give an example of a good URI.**

https://sea-of-cheap-crap-international.com/orders // Good

https://sea-of-cheap-crap-international.com/create-order // Avoid

**7. What does it mean to have a ‘chatty’ web API? Is 
this a good or a bad thing?**

A chatty API is one that requires customers to do more than a single call to perform a single, common operation. Chatty APIs can slow down the system ultimately meaning that it is not a good characteristic for an API to have.

**8. What status code does a successful GET request return**?

HTTP status code 200 (OK).

**9. What status code does an unsuccessful GET request 
return?**

- If the server cannot match any of the media type(s) listed, it should return HTTP status code 406 (Not Acceptable).

- If the resource cannot be found, the method should return 404 (Not Found).

- If the server indicates that this is a partial response the method returns HTTP status code 206. 


**10. What status code does a successful POST request return?**

If a POST method creates a new resource, it returns HTTP status code 201 (Created). 

**11. What status code does a successful DELETE request return?**

If the delete operation is successful, the web server should respond with HTTP status code 204 (No Content),

`[READING-SOURCE] => (https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design)`





## Things I Want To Learn More About

* What are some APIs available that could be useful to me for creating projects that I am interested in?
* What is the difference between APIs and SDKs?
* What is the purpose of the HEAD method of RESTful web services?
* What is the purpose of the OPTIONS method of RESTful web services?
* What are the disadvantages of REST web services?