latency: the time taken for data traveling for end to end. e.g. from one client to server. 


typical latency values

typically latency will be in ms(millisecomds). and network latency can be calculated using the formula:

latency = distance / speed

latency means network delay+computaion delay+processing delay+queueing delay


for reducing the latency we can use cahing and cdn here cahing means storing the requested response of client in cache memory so that next time if the same client request for the same response, it can be served from the cache memory itself and it will be faster than the original response from the server.

typical latency values (round trip time):

LAN:1 ms

WAN:100 ms

and cdn can reduce the latency by serving the response from the nearest server. e.g. if the client is in india and server is in usa, then cdn will serve the response from the nearest server to the client.
and cdn means content delivery network. e.g. when we open youtube.com in india, it will serve the response from the nearest server to the client, which can be in india or nearby. this reduces the latency.
