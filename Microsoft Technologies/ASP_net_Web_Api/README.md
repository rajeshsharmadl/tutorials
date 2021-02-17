# ASP.net Web API

It is a framework for building restful APIs based on http protocol and has been developed on top of Microsoft dotnet framework. However, non restful services can also be developed using ASP.net Web API. REST stands for Representational State Transfer and was first introduced in year 2000 by Roy Fielding. It is an architectural pattern which specifies some constrains an application should adhere to.

**Clients**

- Browsers
- Mobile Applications
- Desktop Applications
- IoT

## REST constraints

- Client/Server - It states that client and server applications should be build separately supporting individual evolution of each application.
- Stateless - It states that nothing should be stored on the server related to client. Each request must contain all the necessary information for the server to process.
- Cacheable - It states that server should be able to cache data which is not changed frequently. E.g. product list in a departmental store does not change so often and can be cached for a time duration during which client will get the cached data avoiding make database request.
- Uniform Interface - It states that each resource should be accessible using a single URI (uniform resource identifier) in turn
