# Reading 09

## Review: High-level HTTP

Bas h for programs and processes and in general files 

HTTP is Hypertext Transfer Protocol

5 steps in a HTTP requests:

Step 1: Local Processing

Browser extracts the "scheme"/protocol

Browser has the intended hostname for the request, it needs to resolve an IP address

Browser will then look through its own cache of recently requested URLs, the operating system’s cache of recent queries, your router’s cache, and your DNS cache

Step 2: Resolve an IP

If the cache lookup fails, your browser fires off a DNS request using UDP

DNS request contains the preconfigured IP for your DNS server and your return IP in its header

UDP is a lightweight protocol, but the tradeoff is that it offers no guarantees in terms of delivery, and there is no acknowledgement other than a response being sent and received

Request will now have to travel many network devices to reach its target DNS server, looking for shortest path to destination 

Request arrives at your configured DNS server, the server looks for the address associated with the requested hostname, response sent if found, target IP required 

Step 3: Establish a TCP Connection

Key differences between TCP and UDP is that TCP ensures delivery and ordered data transmission; done by a sequence number for every byte sent

CP connections are opened using what’s known as a three-way handshake; server must already be "listening" on a port, performing a passive open, after which the client can initiate an active open

Step 4: Send an HTTP Request

Request line" is simply a line that indicates the HTTP method, the resource being requested, and the protocol version

Using TCPs sequence number, the server can ensure it receives the whole request, in the correct order

The server receives the request, processes it, and finds the resource being requested, it generates an HTTP response

Once the response is generated, the server responds to the request

Step 5: Tearing Down and Cleaning Up

Response has been fully delivered, the client sends a FIN packet at the TCP level, to which the server responds with an ACK, and then generally sends a FIN of its own, which the client responds to with its own ACK signal.

Browser begins processing what it has received

(references: https://dev.to/dangolant/things-i-brushed-up-on-this-week-the-http-request-lifecycle-)

## Java HTTP Request example

HTTP request processed by built-in Java class HttpUrlConnection

Disadvantage is the code can be more cumbersome than other HTTP libraries and that it does not provide more advanced functionalities such as dedicated methods for adding headers or authentication

To create an HttpUrlConnection instance use the openConnection() method of the URL class

HttpUrlConnection class is used for all types of requests by setting the requestMethod attribute to one of the values: GET, POST, HEAD, OPTIONS, PUT, DELETE, TRACE

To add parameters we have to set the doOutput property to true, then write a String of the form param1=value¶m2=value to the OutputStream

Adding headers to a request can be achieved by using the setRequestProperty() method

To read the value of a header from a connection, we can use the getHeaderField() method

To set the timeout values, we can use the setConnectTimeout() and setReadTimeout() method

To enable or disable automatically following redirects for a specific connection use the setInstanceFollowRedirects() method with true or false parameter

Reading the response of the request can be done by parsing the InputStream of the HttpUrlConnection instance

(references: https://www.baeldung.com/java-http-request)