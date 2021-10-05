# What I've Learned at the 8th lecture of 401 code...

## The HTTP Request Lifecycle

 **Step 1: Local Processing**

This request is being made by a browser, as opposed to cURL, an API client like Postman, or some other app.

  - The browser extracts the "scheme"/protocol (we have established that this will be HTTP), host (www.example.com),
 and optional port number, resource path, and query strings that are specified in the form <protocol>://<host><:optional port>/<path/to/resource><?query>. An example is |http|://|www.example.com||:5000||/mainpage||?query=param&query2=param2|

 - The browser will then look through its own cache of recently requested URLs, the operating system’s cache of recent queries, your router’s cache, and your DNS cache.

 **Step 2: Resolve an IP**             
 A sequence that includes many steps, and includes failovers if the first request fails to return an address.

 - If the cache lookup fails (we will assume it does), the browser fires off a DNS request using UDP3. The DNS request contains the preconfigured IP for the DNS server and the return IP in its header.

 - The request will now have to travel many network devices to reach its target DNS server.  

 - Once the request arrives at the configured DNS server, the server looks for the address associated with the requested hostname. If it finds one, it sends a response. 

 **Step 3: Establish a TCP Connection**

**TCP:**  which is a transport layer protocol like UDP, the client must open a TCP connection.

  - One of the key differences between TCP and UDP is that TCP ensures delivery and ordered data transmission. 


 **Step 4: Send an HTTP Request**

  - The request is made up of a "request line", request header, and a body.

  - The "request line" is simply a line that indicates the HTTP method, the resource being requested, and the protocol version.

  - Once the HTTP request is sent, it follows a similar routing procedure as the one discussed earlier, with the difference being that using TCPs magic sequence number powers, the server can ensure it receives the whole request, in the correct order.

 - Once the server receives the request, processes it, and finds the resource being requested, it generates an HTTP response. 

 - Once the response is generated, the server responds to the request. At the TCP layer, the client receives the first data packet, the first byte of which should contain the HTTP response header. 

 **Step 5: Tearing Down and Cleaning Up**

 - Once the response has been fully delivered, the client sends a FIN packet at the TCP level, to which the server responds with an ACK, and then generally sends a FIN of its own, which the client responds to with its own ACK signal.

 - At this point, your browser begins processing what it has received. If it is an image, data, or other media file that is being consumed by some application inside the browser, a variety of things can happen.