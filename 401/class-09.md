# The HTTP Request Lifecycle

## Step 1: Local Processing

1. Your browser extracts the "scheme"/protocol, host 
and optional port number, resource path, and query strings that are specified in the form
<protocol>://<host><:optional port>/<path/to/resource><?query>.


2. Now that the browser has the intended hostname for the request, it needs to resolve an IP address1. The browser will then look through its own cache of recently requested URLs, the operating system’s cache of recent queries, your router’s cache, and your DNS cache.


## Step 2: Resolve an IP

if the request is successful : 

If the response makes it back, the requesting client now has a target IP. 

if not : 

1. If the cache lookup fails , your browser fires off a DNS request using UDP3.

2. Your request will now have to travel many network devices to reach its target DNS server.

3. Once your request arrives at your configured DNS server, the server looks for the address associated with the requested hostname.


## Step 3: Establish a TCP Connection

* One of the key differences between TCP and UDP is that TCP ensures delivery and ordered data transmission. 

 The connection has  established a random, sequential sequence11 for each direction of communication (client->server, server->client), allowing for bidirectional, concurrent communication along the connection, which is also known as full duplex communication.

 ## Step 4: Send an HTTP Request


1. The request is made up of a "request line", request header, and a body.

2. Once the HTTP request is sent, it follows a similar routing procedure as the one discussed earlier, with the difference being that using TCPs magic sequence number powers, the server can ensure it receives the whole request, in the correct order.

3. Once the server receives the request, processes it, and finds the resource being requested, it generates an HTTP response

4. Once the response is generated, the server responds to the request. 

## Step 5: Tearing Down and Cleaning Up

1. Once the response has been fully delivered, the client sends a FIN packet at the TCP level, to which the server responds with an ACK, and then generally sends a FIN of its own, which the client responds to with its own ACK signal

2. At this point, your browser begins processing what it has received



# Do a Simple HTTP Request in Java


## HttpUrlConnection

The HttpUrlConnection class allows us to perform basic HTTP requests without the use of any additional libraries.

## Creating a Request

The HttpUrlConnection class is used for all types of requests by setting the requestMethod attribute to one of the values: GET, POST, HEAD, OPTIONS, PUT, DELETE, TRACE.


## Adding Request Parameters

If we want to add parameters to a request, we have to set the Output property to true, then write a String of the form param1=value¶m2=value to the Output Stream of the HttpUrlConnection instance.

## Setting Request Headers

Adding headers to a request can be achieved by using the setRequestProperty() method.



## Configuring Timeouts

HttpUrlConnection class allows setting the connect and read timeouts.

To set the timeout values, we can use the setConnectTimeout() and setReadTimeout() methods.

## Handling Cookies

The java.net package contains classes that ease working with cookies such as CookieManager and HttpCookie.



 ## Handling Redirects

 We can enable or disable automatically following redirects for a specific connection by using the setInstanceFollowRedirects() method with true or false parameter.

 ## Reading the Response

 Reading the response of the request can be done by parsing the InputStream of the HttpUrlConnection instance.

To execute the request, we can use the getResponseCode(), connect(), getInputStream() or getOutputStream() methods.

## Reading the Response on Failed Requests

Reading the RIf the request fails, trying to read the InputStream of the HttpUrlConnection instance won't work.

## Building the Full Response

It's not possible to get the full response representation using the HttpUrlConnection instance.






