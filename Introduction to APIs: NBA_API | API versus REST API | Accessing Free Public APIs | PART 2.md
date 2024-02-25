Hello Dears,

In the Introduction to APIs series, so far, we in the [**PART 1**](https://www.kaggle.com/discussions/general/479591#2668341) learned about API and its structures. Before starting this part, please read PART 1 if API is something new to you.

**In this part we are going to learn the following:**
- NBA_API
- API vs REST API
- Accessing free public APIs

## **NBA_API**
The "nba_api" offers programmatic access to a wealth of **National Basketball Association (NBA)** data, including detailed player stats, team insights, and game outcomes, enabling developers to fetch basketball-related information efficiently. Its use should comply with data usage policies. The NBA_API aims to assist developers in creating applications that need basketball-related data without having to scrape the information from the official NBA site or other sources.

## **API vs REST API**
An Application Programming Interface (API) and a Representational State Transfer API (REST API) are interconnected concepts with notable differences. Here's an overview:
| Feature | API | REST API |
| --- | --- | --- |
| Full form | Application programming interface | Representational state transfer API |
| Definition | 	A set of protocols and tools for building software applications. It defines how different software components should interact. | A specific type of web API that follows the principles of representational state transfer (REST). It is an architectural style for designing networked applications. |
| Scope | A broader term encompassing various types of interfaces | Specifically refers to APIs following the principles of REST architecture |
| Communication | API communication methods can vary (Remote procedure call (RPC), Simple objects access protocol (SOAP), and so on) | Uses standard HTTP methods (GET, POST, PUT, DELETE) for communication |
| Architectural style | No specific architectural style | Follows the REST architectural style |
| Data format | Can use different data formats (JSON, XML, and so on) | Typically uses lightweight data formats, commonly JSON, for data exchange |
| URI | Resource identification methods may vary | Resources identified by URIs, each with multiple representations |
| Usage | Used in various contexts (web development, libraries, operating systems, and so on) | Primarily used for web services and web-based applications |


## **Accessing Free Public APIs**
To integrate a public API into your Python script, you must identify the API endpoint's URL. Discovering the URL for a public API is achievable by consulting the list available on the specified GitHub repository.

- Visit the "public-apis" GitHub repository at `[https://github.com/public-apis/public-apis](https://github.com/public-apis/public-apis)`.
- Scroll through the API directory to find the service you wish to use.
- Identify the base URL for the API from the "API" column in the repository's table.
- Check the "Auth" and "HTTPS" columns for any authentication or protocol specifics.
- Utilize the base URL in your Python code with the `requests` library to interact with the API.

After obtaining the API's URL, employ the `requests` library in Python to execute HTTP requests and obtain data from the API. For instance, to fetch information from the FishWatch API, the following snippet could be used in your code:

```python
import requests  # For HTTP requests.
import json  # For JSON data manipulation.

# API endpoint URL for fish species information.
url = "https://www.fishwatch.gov/api/species"

# Perform HTTP GET request and store response.
data = requests.get(url)

# Convert JSON response to a Python dictionary.
results = json.loads(data.text)
```
Keep in mind that the exact endpoint you need may vary by API, so consulting the API's documentation is crucial for understanding its usage.

I already published a notebook showing how to access public API. **Please check the following notebook to get some hands-on experience. **
>[**Application Programming Interface (API)**](https://www.kaggle.com/code/tanvirnwu/application-programming-interface-api?scriptVersionId=164232017)

## Extras
While discussing APIs, we need to know some additional topics as follows:
- **Rate Limiting:** Many APIs have rate limits to prevent abuse. Understanding and handling these limits is crucial for avoiding service disruptions.
- **API Keys:** Some APIs require you to register and use an API key for requests. This key is essential for tracking and controlling API usage.
- **Data Formats:** While JSON is common, APIs may offer data in other formats like XML. Knowing how to handle different data formats can be beneficial.
- **Error Handling:** Learn how to interpret and handle API errors gracefully in your code to enhance the robustness of your application.
- **Security Practices:** When using APIs, especially with authentication, it's important to follow security best practices to protect sensitive information.
- **Caching Responses:** To improve performance and reduce API calls, consider caching responses for frequently requested data.
- **Asynchronous Requests:** For applications that require high performance, learn to make asynchronous API calls to avoid blocking your application's execution flow.
- **API Versioning:** APIs evolve, and versions change. Keep an eye on version updates to ensure your application remains compatible.
- **Community and Support:** Engaging with the community and seeking support can be helpful, especially for popular APIs where forums and discussion groups can provide valuable insights.
- **Compliance and Legal Considerations:** Be aware of any legal implications or compliance requirements related to the data you access via APIs, especially for commercial projects.


So far we studied:
- [Introduction to APIs: How APIs Work? | Structures of API | PART 1](https://www.kaggle.com/discussions/general/479591#2668341) 
- [Introduction to APIs: NBA_API | API versus REST API | Accessing Free Public APIs | PART 2](https://www.kaggle.com/discussions/general/479591#2668341)
-  [Application Programming Interface (API)](https://www.kaggle.com/code/tanvirnwu/application-programming-interface-api?scriptVersionId=164232017)


***Please let me know if you are interested to know more about APIs and need more hands-on examples in Python. Currently, I am also learning the basics of APIs. So, I am also excited to share with you guys if I get some support from you.***
