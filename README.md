# discoveryServer
Springboot Discovery Server implmentation using Eureka for microservices registration and discovery.

Service clients on start-up register and on shutdown de-register with Eureka Server using the configuration in Eureka Client service.

EurekaServer configuration isn't required to be resigtered and this is achieved with configuration on Discovery server set as:

client:
   registerWithEureka: false
   fetchRegistry: false

The start-up class annotation @EnableEurekaServer identifies the service as discovery Server.
