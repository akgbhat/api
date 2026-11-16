# API
> **API** stands for **Application Programming Interface**
<li> A way for software programs to communicate and exchange information.</li>
<li> They act as invisible connectors that make modern software work together.</li>

## Topics
- [Model](#model)
- [Functions of API](#functions-of-api)
- [Web APIs](#web-apis)
    - [Types of Web APIs](#types-of-web-apis)
    - [How Web APIs work](#how-web-apis-work)


## Model
Think of a restaurant:
- **You (the client)** place an order from the menu (**request**).
- **The kitchen (the server)** prepares it using its *own resources*.
- **The waiter** delivers the *response* back to your table.

## Functions of API

* Data Sharing:
> apps exchange information in real time. Eg: weather apps
* Service Integration:
> connect payment processors, mapping tools, or messaging platforms into your own product without building them from scratch.
* Automation:
>trigger actions automatically acrss systems. Prevents isolation.

API helps to avoid the building every capability from scratch - it lets teams share **functionality** and **robust building** by connecting <u>existing services</u>.

## Web APIs

- They allow you to access over the internet using HTTP. 
- They let apps send requests to **remote services** and get data/functionality back.

### Types of Web APIs
1. SOAP API
- uses **XML** to exchange data.
- more rigid and verbose - suited for complex operations that require strict contract.
- used in enterprise and legacy systems.

2. RESTful APIs
- uses **HTTP** methods like **GET**, **POST**, **PUT**, and **DELETE**.
- works with URLs that represent resources.
- each request is handled independantly and easy to use with web technologies.

## How Web APIs work
> Every interaction with web API follows the same pattern: Send a request to specific URL <-> Receive a response on data or functionality of the system.

### Endpoints
Its a specific URL that represents a resource or action in an API - address the rquest is send to.

Each **endpoint** typically maps to a particular piece of data or functionality. They follow predictable patterns organized by resource type, making APIs easier to navigate.

Example: `https://myurl.com/tasks` might return all tasks, while `https://myurl.com/tasks/1` returns just the task with ID `1`.

> Model - **destination**

### HTTP methods
- it tells the API what action you want to perform on an endpoint.

Endpoints --> <italics>what</italics> you're interacting with
methods --> <italics>how</italics>

| Method | Action | Example |
| --- | --- | --- |
| GET | Retrieve data | Get a list of tasks |
| POST | Submit new data | Create a new task |
| PUT | Update existing data | Mark a task as complete |
| DELETE | Remove data | Delete a task |

### Request

- its the message send to an API aking for data or an action.
- every request contains the same core parts:
1. Endpoints: tells the API which <bold>resource</bold> you want to interact with. [The target url]
2. Method: action you want to take -- GET, POST, PUT, or DELETE.
3. Headers, Parameters and Body: authentication tokens in headers, filters as query parameters, or the data payload in the request body (for POST and PUT requests).

### Respsonse
- It tells you whether the request succeeded and returns any relevant data

1. Status Code: success/failure -- 200 OK, 201 Created, 404 Not Found, 500 Server Error.
2. Body: The data returned by the API, usually formatted as JSON.
3. Headers: Metadata like content type, rate limit info, or caching instructions.





