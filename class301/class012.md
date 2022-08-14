# Readings: CRUD

## [Status Codes Based On REST Methods](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)

In your own words, describe what each group of status code represents:

100’s = they will tell you information about the request status

200’s = these are request success responses but it doesn't mean that the request was successfully proccessed rather all the validation requirements met.

300’s = these are redirection codes meaning that when a client requests for the info, at the time it is not available.

400’s = these are client error codes when the response to the server is unresponsive.

500’s = these are server error codes when the server has overwhelming amounts of traffic or unreachable servers

What is a status code 202?

- Accepted used for asynchronous processing

What is a status code 308?

- permanent redirect when the current url is no longer available and wants the client to use another url.

What code would you use if an update didn’t return data to a client?

- 300

What code would you use if a resource used to exist but no longer does?

- 204

What is the ‘Forbidden’ status code?

- where the client is not authorized to the backend of the application

## [Build A REST API With Node.js, Express, & MongoDB - Quick ](https://www.youtube.com/watch?v=fgTGADljAeg)

Why do we need to pull our MongoDB database string out of our server and put it into our .env?

-

What is middleware?

-

What does app.use(express.json()) do?

-

What does the /:id mean in a route?

-

What is the difference between PUT and PATCH?

-

How do you make a default value in a schema?

-

What does a 500 error status code mean?

-

What is the difference between a status 200 and a status 201?

-
