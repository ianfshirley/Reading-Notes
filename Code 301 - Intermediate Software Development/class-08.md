## APIs

### API Design Best Practices

1. What does REST stand for?
- Representational State Transfer
2. REST APIs are designed around a ____.
- resource
3. What is an identifier of a resource? Give an example.
- it's a URI that uniquely identifies that resource. It's what comes after the slash on a URL
4. What are the most common HTTP verbs?
- GET, POST, PUT, PATCH, DELETE
5. What should the URIs be based on?
- nouns (the resource)
6. Give an example of a good URI.
- https://adventure-works.com/orders (good) vs. ....works.com/create-order (bad)
7. What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?
- It's bad. Too many requests, creating a bigger load.
8. What status code does a successful GET request return?
- 200
9. What status code does an unsuccessful GET request return?
- 404
10. What status code does a successful POST request return?
- 201
11. What status code does a successful DELETE request return?
- 204

### Sources

[API Design Best Practices](https://learn.microsoft.com/en-us/azure/architecture/best-practices/api-design)<br>
[RegExr](https://regexr.com/)<br>
[Regex Tutorial](https://medium.com/factory-mind/regex-tutorial-a-simple-cheatsheet-by-examples-649dc1c3f285)<br>
[Regex 101](https://regex101.com/)<br>