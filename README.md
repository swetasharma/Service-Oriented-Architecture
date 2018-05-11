# Service-Oriented-Architecture

Service oriented architecture is all about how to build, use and combine services.

You -> Car Service -> Car Maintenance service
    -> Meal Service -> Food Supply Service
    -> Laundry Service -> Appliance Maintenance Service

Bringing the concept of services into software. Instead of building large software suites that do everything.
Once service oriented archotecture is in place, it is very powerful because it provides modularity, extensibilitya and code reuse. Applications can be built by combining services. New services can be created by combining by combining exisitng services or new services can be created from the ground up or by adding interfaces to existing code.

Service Principles / Best Practices:

1. Modular : Services should be modular and loosely coupled. In object oriented programming, loose coupling is achieved by only exposing the relevant elements of a class or components to its clients. In service oriented architecture, requests are made by passing communcation to the service in way that aligns with its interface. The service performs necessary operations then passes back a communication containing the results of the service or a confirmation that the requst was fulfilled.
2. Composable: 
3. Platform and Language independent: a sverice which is coded in java can be used by a servcie requester coded in Ruby.Platform and language indepedebce is achieved by following communication standards and protocols.
4. Self Describing:
5. Self Advertising:


The relationship bwetween web browser nad wb server is a client server relationship. both the request and responce are messages conveyed in HTTP. a communication protocol that both the web browser and web server understand.
static page are stored on the wen server, while dynamic pages are built by the web server when they are requested.
The desktop appications are run and are stored locally on your computer, whereas web applications run in your web browser, and are stored on a remote web server.
Web applications are platform indepwendent, meaning that the application will run on any operating syetem, provided that a compatible web browser is installed. web applicaiton almost always require users to have internet access because information is communicated over HTTP


Static web page: Web browser | Web server | HTML Documents
Dynamic web page : Web Browser | Web server | Application Server | Database.




HTTP:(Hypertext transport protocol)
Universal Resource Identifiers:
All URLs are URIs, but not all URIs are URLs.


HttP was designed to facilitate the use of hypertext and to support the communication of documents and resources expressed in HTML. Now of course we use hyperlinks to link otgretehr multimedai resources such as images, videos , GIF's texts, and audio or documensts caontianing any combination of these.


HTTP is built on top of another protocol called the transmission control protocol TCP. 
HTTP messages are sent and received through TCP ports. 

when your browser accesses a URI that starts wITH HTTP, A connection between your web browser and a web server is opened on TCP port 80, the default port for HTTP messages.

HTTP is built upon a client/server design. when a client makes a request to a server, this opens a TCP connection between the client and server for them to communicate.


Below information must be included in every HTTP request from a client:

Accept Header(This tells ther server what kind of content will be accepted as a response. This could  be HTML for example, or JSON) and Host Header(this contains a domain name or an IP address)

We need to learn about URL-encoding. HTTP limits the characters used in URIs, request queries and request bodies to be ASCII. Special or unsafe characters, like space or unicode, require you to encide these characters.

space is a special case in that there are two ways to encode it We can encode a space using the percent sign followed by 20 or a plus sign.


What it means for HTTP to be stateless and consequences of statelessness:
It means that the relationship between requests is not perserved. For exxample, if you are browsing an online shopping website and cllicking on items, the HTTP protocol does not keep track of which items you have previously clicked.
A website can use HTTP cookies to track the behavior of shoppers on their site. 
The first time a client makes a request, the site gives them an HTTP cookie to store informaiton about the clients browsing session. The cooie is stored by the cllient and uopdated by the server each time the client makes a request  to the server.This allows a server to store state information about interactions with this client, which can be useful for tracking purposes. 



Remote Procedure Call:


REST (Representational state transfer):

It is used in Distributed applications by using HTTP to send messgaes to communicate between components.In the moste basoc terms, REST is a client server architecture based on request reponse design. Aspecific feature of REST is that communication is resource based. REST has five constraints:
1. REST is a client-server architecture. (allows development of client and the server to occur independemtly of each other )
2. REST is a layered system.
3. Interaction must be stateless.(server does not save information about the current client state or previous request made by the client each request is independent of each other and must contain all  necessary information for the server to understand and respond to the request. This constraint improves performance of web servcies becuase the server does not have to store any information about the current states of clients in the system. example if authentication is needed by server for a client to have access to data, the client must send that authentication information in every request).






















































