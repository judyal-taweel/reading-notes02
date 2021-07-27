# WebSocket

- its guild about how to build interactive web applications that send and receive messages between client and the server.
- we use WebSocket to build interactive web application .
- we will use STOMP messaging with Spring to create an interactive web application .
- STOMP is a subprotocol operating on top of the lower-level WebSocket.
we will use STOMP dependencies
dependencies {

	implementation 'org.springframework.boot:spring-boot-starter-websocket'
}

Should I Use WebSocket?
With all the design considerations surrounding the use of WebSocket, it is reasonable to ask, "When is it appropriate to use?".
The best fit for WebSocket is in web applications where the client and server need to exchange events at high frequency and with low latency. Prime candidates include, but are not limited to, applications in finance, games, collaboration, and others. Such applications are both very sensitive to time delays and also need to exchange a wide variety of messages at a high frequency.
For other application types, however, this may not be the case. For example, a news or social feed that shows breaking news as it becomes available may be perfectly okay with simple polling once every few minutes. Here latency is important, but it is acceptable if the news takes a few minutes to appear.
Even in cases where latency is crucial, if the volume of messages is relatively low (e.g. monitoring network failures) the use of long polling should be considered as a relatively simple alternative that works reliably and is comparable in terms of efficiency (again assuming the volume of messages is relatively low).
It is the combination of both low latency and high frequency of messages that can make the use of the WebSocket protocol critical. Even in such applications, the choice remains whether all client-server communication should be done through WebSocket messages as opposed to using HTTP and REST. The answer is going to vary by application; however, it is likely that some functionality may be exposed over both WebSocket and as a REST API in order to provide clients with alternatives. Furthermore, a REST API call may need to broadcast a message to interested clients connected via WebSocket.
The Spring Framework allows @Controller and @RestController classes to have both HTTP request handling and WebSocket message handling methods. Furthermore, a Spring MVC request handling method, or any application method for that matter, can easily broadcast a message to all interested WebSocket clients or to a specific user.