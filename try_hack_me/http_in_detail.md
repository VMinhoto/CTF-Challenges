# URL
https://tryhackme.com/room/httpindetail
# Category
Fundamentals
# Concept
Learn about Http
# Method of solve
## Task 1
* HTTP is what's used whenever you view a website, HTTPS is HTTP but encrypted
* Anwers are: `HyperText Transfer Protocol`, `secure` and `THM{INVALID_HTTP_CERT}`
## Task 2
### URLS

  
<img width="1140" height="270" alt="34ad66d8b90aaaa35f9536d3b152ea97" src="https://github.com/user-attachments/assets/1a5f9562-5d30-4283-add1-32ef3d9108ea" />

* Learn about URLs

  * Scheme: This instructs on what protocol to use for accessing the resource such as HTTP, HTTPS, FTP (File Transfer Protocol). User: Some services require authentication to log in, you can put a username and password into the URL to log in.Host: The domain name or IP address of the server you wish to access.

  * Port: The Port that you are going to connect to, usually 80 for HTTP and 443 for HTTPS, but this can be hosted on any port between 1 - 65535.

  * Path: The file name or location of the resource you are trying to access.

  * Query String: Extra bits of information that can be sent to the requested path. For example, /blog?id=1 would tell the blog path that you wish to receive the blog article with the id of 1.

  * Fragment: This is a reference to a location on the actual page requested. This is commonly used for pages with long content and can have a certain part of the page directly linked to it, so it is viewable to the user as soon as they access the page.


### Request
```
GET / HTTP/1.1

Host: tryhackme.com
User-Agent: Mozilla/5.0 Firefox/87.0
Referer: https://tryhackme.com/

```
* Request Example
  
  * Line 1: This request is sending the GET method ( more on this in the HTTP Methods task ), request the home page with / and telling the web server we are using HTTP protocol version 1.1.

  * Line 2: We tell the web server we want the website tryhackme.com

  * Line 3: We tell the web server we are using the Firefox version 87 Browser

  * Line 4: We are telling the web server that the web page that referred us to this one is https://tryhackme.com

  * Line 5: HTTP requests always end with a blank line to inform the web server that the request has finished.
 
### Response

```
HTTP/1.1 200 OK

Server: nginx/1.15.8
Date: Fri, 09 Apr 2021 13:34:03 GMT
Content-Type: text/html
Content-Length: 98


<html>
<head>
    <title>TryHackMe</title>
</head>
<body>
    Welcome To TryHackMe.com
</body>
</html>

```
* Response example
  * Line 1: HTTP 1.1 is the version of the HTTP protocol the server is using and then followed by the HTTP Status Code in this case "200 OK" which tells us the request has completed successfully.

  * Line 2: This tells us the web server software and version number.

  * Line 3: The current date, time and timezone of the web server.

  * Line 4: The Content-Type header tells the client what sort of information is going to be sent, such as HTML, images, videos, pdf, XML.

  * Line 5: Content-Length tells the client how long the response is, this way we can confirm no data is missing.

  * Line 6: HTTP response contains a blank line to confirm the end of the HTTP response.

  * Lines 7-14: The information that has been requested, in this instance the homepage.
 
### Answers
* `HTTP/1.1`
* `Content Length`

## Task 3
* GET Request: This is used for getting information from a web server

* POST Request: This is used for submitting data to the web server and potentially creating new records

* PUT Request: This is used for submitting data to a web server to update information

* DELETE Request: This is used for deleting information/records from a web server.

* Answers are: `POST`, `PUT`, `DELETE`, `GET`

## Task 4

Status codes:

| Status Code Range | Description |
| ----------- | ----------- |
| **100-199 - Information Response** | These are sent to tell the client the first part of their request has been accepted and they should continue sending the rest of their request. These codes are no longer very common. |
| **200-299 - Success** | This range of status codes is used to tell the client their request was successful. |
| **300-399 - Redirection** | These are used to redirect the client's request to another resource. This can be either to a different webpage or a different website altogether. |
| **400-499 - Client Errors** | Used to inform the client that there was an error with their request. |
| **500-599 - Server Errors** | This is reserved for errors happening on the server-side and usually indicate quite a major problem with the server handling the request. |

* Answers are: `201`, `404`, `503`, `401`

* ## Task 5
* The answers are: `User-Agent`, `Contet-Type`,`Host`

## Task 5
* Answer is `Set-Cookie`

## Task6
* Use the postman like interface to find the flags

