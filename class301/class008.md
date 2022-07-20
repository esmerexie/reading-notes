# Readings: APIs

All answers to the questions can be referred from [here](https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design)

## API Design Best Practices

What does REST stand for?

- Representational State Transfer

REST APIs are designed around a ____.

- resouces

What is an identifier of a resource? Give an example.

- URI that uniquely identifies that resource

```http

https://adventure-works.com/orders/1

```

What are the most common HTTP verbs?

- Get, POST, PUT, PATCH, and DELETE

What should the URIs be based on?

- Resource

Give an example of a good URI.

 ```html
 https://adventure-works.com/orders 
 ```

What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?

- A chatty web api usually means the amount of web requests your server. And a chatty web api usually exposes a large number of small resources.

What status code does a successful GET request return?

- 200 (ok)

What status code does an unsuccessful GET request return?

- 404 (Not Found)

What status code does a successful POST request return?

- 201 (Created)

What status code does a successful DELETE request return?

- 204 (No Content)

## Things I want to know more about
