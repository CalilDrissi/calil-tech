---
title : "Guide to REST APIs"
description: Explore the basics of APIs, what we can use them for, how to design them and various ways we can protect them.
date : 2021-04-15T23:04:59Z
author : "Calil Drissi"
image: https://f000.backblazeb2.com/file/Calilz-refs-bucket/api.png
authorImage: /images/whoami/author-3.jpg
categories:
- Back-End
- Architecture 
draft: false
enableToc: true
enableTocContent: false
pinned: false
---

![restApi](/images/feature2/rest-api.png "Restapi")

In the age of distributed systems and web services the REST API design - REST, also called RESTful (Representational State Transfer) API (Application Programming Interface) - has become a central technology for the modern web. Built on top of established protocols mostly http for Web apis. REST APIs are lightweight and flexible making system to system integrations, data sharing & interactivity much more simpler and concise.


## What is a REST API?

A REST API is first of all an architectural style for handling applications interactivity and data exchange usually in JSON OR XML between a web server and a client such as a browser, a mobile app etc...

To understand it well let's define its two parts:

**API** is an application programming interface, it allows one piece of software to talk to another using a predefined set of rules with the objective of performing functionalities built around sharing data between programs. In our case The developer creates the API on the server to make it interact with the client side.


**REST** defines the set of rules of the API architecture that is based on  a stateless request/response cycle, meaning you should be able to receive a piece of data when you link to a specific URL and that every request happens in complete isolation. Each URL endpoint is commonly referred to as a **request** while the data sent back to is referred to as a **response.**


## How Do REST APIs work?

Although flexibility is a big advantage of REST API design, that same flexibility makes it easy to design an API that’s broken or performs poorly. For this reason, professional developers share best practices in REST API specifications.

The OpenAPI Specification (OAS) establishes an interface for describing an API in a way that allows any developer or application to discover it and fully understand its parameters and capabilities - available endpoints, allowed operations on each endpoint, operation parameters, authentication methods, and other information. The latest version, OAS3 (link resides outside IBM), includes with hands-on tools, such as the OpenAPI Generator, for generating API clients and server stubs in different programming languages.

Securing a REST API also starts with industry best practices, such as using hashing algorithms for password security and HTTPS for secure data transmission. An authorization framework like OAuth 2.0 (link resides outside IBM) can help limit the privileges of third-party applications. Using a timestamp in the HTTP header, an API can also reject any request that arrives after a certain time period. Parameter validation and JSON Web Tokens are other ways to ensure that only authorized clients can access the API.

## REST design principles?

At the most basic level, an API is a mechanism that enables an application or service to access a resource within another application or service. The application or service doing the accessing is called the client, and the application or service containing the resource is called the server.

Some APIs, such as SOAP or XML-RPC, impose a strict framework on developers. But REST APIs can be developed using virtually any programming language and support a variety of data formats. The only requirement is that they align to the following six REST design principles - also known as architectural constraints:

1. **Uniform interface.** All API requests for the same resource should look the same, no matter where the request comes from. The REST API should ensure that the same piece of data, such as the name or email address of a user, belongs to only one uniform resource identifier (URI). Resources shouldn’t be too large but should contain every piece of information that the client might need.

2. **Client-server decoupling.** In REST API design, client and server applications must be completely independent of each other. The only information the client application should know is the URI of the requested resource; it can't interact with the server application in any other ways. Similarly, a server application shouldn't modify the client application other than passing it to the requested data via HTTP.

3. **Statelessness.** REST APIs are stateless, meaning that each request needs to include all the information necessary for processing it. In other words, REST APIs do not require any server-side sessions. Server applications aren’t allowed to store any data related to a client request.

4. **Cacheability.** When possible, resources should be cacheable on the client or server side. Server responses also need to contain information about whether caching is allowed for the delivered resource. The goal is to improve performance on the client side, while increasing scalability on the server side.

5. **Layered system architecture.** In REST APIs, the calls and responses go through different layers. As a rule of thumb, don’t assume that the client and server applications connect directly to each other. There may be a number of different intermediaries in the communication loop. REST APIs need to be designed so that neither the client nor the server can tell whether it communicates with the end application or an intermediary.

6. **Code on demand (optional).** REST APIs usually send static resources, but in certain cases, responses can also contain executable code (such as Java applets). In these cases, the code should only run on-demand.

## The Anatomy Of A Request?
Anytime a call is made to a server using a REST API, that is considered an API request. And while the outcome happens quickly and quite simply, there is actually a lot that goes into making that request itself.

#### The Endpoint

The endpoint of a REST API is a unique URL that represents an object or group of objects of data. Each API request has its own endpoint, which is what the HTTP client is directed at in order to interact with data resources.

#### The Method

HTTP methods (which will be explained in further detail below) are an integral part of a RESTful API request. These methods – GET, POST, PUSH, PATCH, and DELETE – correspond to create, read, update, and delete resources.

#### The Headers

REST headers contain information that represent metadata associated with every single REST API request. A REST header indicates the format of the request and response, and provides information about the status of the request.

#### The Data

A REST API request also consists of data (also referred to as a “body”) that usually works with the POST, PUT, and PATCH HTTP commands and contains the information and representation of the resource that will be created.



## HTTP Request Methods

As outlined above, REST APIs are designed to perform requests and receive responses via HTTP functions. These are the five HTTP commands that REST is based on.

#### GET Request

The GET request is a nullipotent command that safely retrieves information. No matter how many times it repeats with identical parameters, the results will always be the same.

#### POST Request

The POST request is used to request the origin server accepts the entity enclosed in the request as a new subordinate of the resource. It can also update an existing entity.

#### PUT and PATCH Requests

The PUT request is an idempotent command that can create, update, or replace an entity. The PATCH request is also an idempotent command, which simply replaces an entity.

#### DELETE Request

The DELETE request is an idempotent command that a resource be removed. One important detail to note is that the resource does not have to be removed immediately; it could also be asynchronous or a long-running request.

## Authentication in a RESTful Api?

There are a few approaches when it comes to REST API authentication. It’s important to note that almost every REST API must have at least some form of authentication. Authentication verifies the credentials of a connection attempt between the sender and receiver. HTTP basic authentication is the simplest way to authenticate a REST API. In this scenario, an HTTP user agent provides a username and a password to verify its identity.

Another option for REST API authentication is using API keys. In this approach, a unique generated value is assigned to every first-time user, so that every additional time that user tries to enter the system, the unique key is used again to prove that they are in fact the same user as before.

The other method is actually a combination of authentication and authorization, called OAuth. In this scenario, a user logs into a system, and then the system requests authentication, normally in the form of a token. Next, the user’s request is forwarded to an authentication server that either allows or rejects the authentication. From there, the token goes back to the user and then to the requester. The token can be checked at any time by the requester and also over time with a specific scope and longevity.

## REST API best practices?

Although flexibility is a big advantage of REST API design, that same flexibility makes it easy to design an API that’s broken or performs poorly. For this reason, professional developers share best practices in REST API specifications.

The OpenAPI Specification (OAS) establishes an interface for describing an API in a way that allows any developer or application to discover it and fully understand its parameters and capabilities - available endpoints, allowed operations on each endpoint, operation parameters, authentication methods, and other information. The latest version, OAS3 (link resides outside IBM), includes with hands-on tools, such as the OpenAPI Generator, for generating API clients and server stubs in different programming languages.

Securing a REST API also starts with industry best practices, such as using hashing algorithms for password security and HTTPS for secure data transmission. An authorization framework like OAuth 2.0 (link resides outside IBM) can help limit the privileges of third-party applications. Using a timestamp in the HTTP header, an API can also reject any request that arrives after a certain time period. Parameter validation and JSON Web Tokens are other ways to ensure that only authorized clients can access the API.


## Conclusion 

APIs are critical in spanning technical and business boundaries to deliver data, capabilities, and services wherever (and whenever) they’re needed, but the design of APIs has shifted to the more lightweight and flexible varieties that are suited for mobile applications and geo-distributed networks.

Because of this approach, REST APIs continue to grow in popularity for mobile apps, social networking sites, and a variety of other offerings. Thousands of enterprises use REST APIs to generate business and grow their services, and REST API adoption will continue as one of the most efficient ways to enable the next generation of business applications.

