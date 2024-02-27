## Introduction
-------
An Application Programming Interface (API) is a set of protocols and tools for building software applications. It acts as a bridge that allows different software programs to communicate. APIs define the methods and data formats developers can use to interact with the software components, whether they are part of the same system or belong to external services. For instance, when we use an app on our phone to check the weather, the app uses an API to request data from a remote server. The API handles this interaction, ensuring that the app can display the information without needing to understand the details of how the server retrieves the weather data. APIs are essential in modern software development, enabling seamless integration and function sharing across diverse platforms and services.

![](https://www.googleapis.com/download/storage/v1/b/kaggle-forum-message-attachments/o/inbox%2F12922590%2F8e90e10d27e9feedf34050a82ab06de9%2FAPI-01.jpg?generation=1708853441263425&alt=media)
-------
## Working Process of APIs
An API is a set of protocols that allows different software applications to communicate. It consists of:

**Endpoints:** Each endpoint, typically a specific URL, represents a distinct function the API provides, like querying a database or posting data.

**HTTP Methods:** These define the type of operation to be executed:
| HTTP Methods | Description |
| --- | --- |
| GET | Retrieves data from server  |
| POST |Submits new data, creating a new entry |
| PUT/PATCH |  Alters existing data |
|DELETE  |  Erases data|


**Headers:** Part of the HTTP request, headers contain metadata such as content type or authentication tokens that provide context for the request.

**Body:** The body of a request might carry data for creating or updating a resource, especially in POST or PUT methods.

```python
<!DOCTYPE html>
<html>
<body>
<h1>My First Heading</h1>
<p>My first paragraph.</p>
</body>
</html>
```


**Status Codes:** The server responds with these codes, which indicate the outcome of the API call, such as 200 for success or 404 for not found. The other status codes are as follows:

| Status Code | Indication | Status Code | Indication |
| --- | --- | --- | --- |
| 1XX | Informational | 4XX| Client Error|
| 100| Everything So Far Is OK | 401| Unauthorized|
| 2XX| Success| 403| Forbidden|
| 200| OK | 404 | Not Found|
| 3XX| Redirection| 500| Server Error|
| 300| Multiple Choices|  501| No Implemented|


**Authentication:** Authentication is a critical feature of many APIs, serving as a gateway to ensure that only vetted users or services have access to specified resources. Standard API authentication methods include API keys, OAuth tokens, and various other secure mechanisms.

**Documentation:** Well-designed APIs are accompanied by thorough documentation. Such documentation provides detailed instructions on utilizing the API, outlines the endpoints available, and describes the expected formats for requests and responses. It also includes guidelines for authentication processes. This information is vital for developers to understand and integrate with the API effectively.

-------
## Structure  of API URLs
An example of the API structure is as follows:
![](https://www.googleapis.com/download/storage/v1/b/kaggle-forum-message-attachments/o/inbox%2F12922590%2F1a2e09683554f48292d42a74224b43bc%2FAPI-02.jpg?generation=1708853589342728&alt=media)

- **Scheme:** The 'scheme' refers to the protocol used for the API communication, in this case, `https://`, denoting secure HTTP access.

- **UniformResource Identifier (URL):** A Uniform Resource Identifier (URI) is a string used to identify a resource on the internet, which can be a name or a resource itself. For example, the string is shown below: 
`https://api.example.com/v1/get/json.xml?parameter1=value1&parameter2=value2 `
represents a URI where various components are specified. A Uniform Resource Locator (URL) is a subset of URI, which provides the location to access a resource on the web. For instance, `https://api.example.com` is the URL portion of the above URI.

- **Route:** The 'route' points to the specific path on the server where the API can be accessed, such as /v1/get/json.xml.

- **Parameters:** Parameters are appended to the URI to provide additional data for the request. In the URI provided, parameter1=value1&parameter2=value2 are the parameters that define the input data for the API request.



----
**So far we studied:**
- [Introduction to APIs: How APIs Work? | Structures of API | PART 1]([https://www.kaggle.com/discussions/general/479591#2668341](https://github.com/tanvirnwu/Basics-of-APIs/blob/main/Introduction%20to%20APIs%3A%20How%20API%20Work%3F%20%7C%20Structures%20of%20API%20%7C%20PART%201.md)) 
- [Introduction to APIs: NBA_API | API versus REST API | Accessing Free Public APIs | PART 2](https://github.com/tanvirnwu/Basics-of-APIs/blob/main/Introduction%20to%20APIs%3A%20NBA_API%20%7C%20API%20versus%20REST%20API%20%7C%20Accessing%20Free%20Public%20APIs%20%7C%20PART%202.md)
- [Application Programming Interface (API)](https://github.com/tanvirnwu/Basics-of-APIs/blob/main/Application%20Programming%20Interface%20(API).ipynb)


--------
Special thanks to [Akansha Yadav](https://www.linkedin.com/in/akansha-yadav-4bb7321a9/)!
