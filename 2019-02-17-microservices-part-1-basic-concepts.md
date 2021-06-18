---
id: 1115
title: 'Microservices Part 1 &#8211; Basic Concepts'
date: 2019-02-17T13:50:22+05:30
author: admin@sciloo.com
layout: post
guid: https://sciloo.com/?p=1115
permalink: /2019/02/17/microservices-part-1-basic-concepts/
colormag_page_layout:
  - default_layout
xyz_smap:
  - "1"
categories:
  - Startups
  - technology
tags:
  - domain driven design
  - microservices
  - Software Architecture
---
### A microservice is an architectural style with small services which are

  1. isolated, 
  2. loosely-coupled 
  3. works on a single concern.
  4. Own their own data
  5. Lightweight communication usually with HTTP Restful API
  6. Built around business capabilities/domain, example below 

DDD (<g class="gr_ gr\_13 gr-alert gr\_spell gr\_inline\_cards gr\_run\_anim ContextualSpelling ins-del multiReplace" id="13" data-gr-id="13">Domain driven</g> design) is the way to go while <g class="gr_ gr\_25 gr-alert gr\_spell gr\_inline\_cards gr\_run\_anim ContextualSpelling ins-del multiReplace" id="25" data-gr-id="25">designig</g> microservices.<figure class="wp-block-image">

![](http://lh5.googleusercontent.com/OlYKfFDflU8_Pjv-ppbq6CtTeV8-J7O-a6PKceZJSLQWaVU4x30Kf63oKlwyaxHonk01lwI5dR8yqSSZvHd8py7PPTlhhoQGTtP94oPNIEOzeCHnB8LSxuSZcqG2sm-OCgVmWZw-) </figure> 

  1. Independently deployable by automated means
  2. Right tech for right problem &#8211; each microservice can be implemented on its own tech

Advantages

  1. Language independent as conform to HTTP Restful
  2. Individual team for each microservice
  3. Scalable
  4. Fault tolerance
  5. Container friendly (docker, kubernete)
  6. Fast iteration for adding code
  7. small development teams, 
  8. shorter development cycles
  9. flexibility in language selection
 10. enhanced service scalability

Disadvantages

  1. Complex interactions &#8211; System + Operational
  2. Overhead of communication across databases and servers
  3. Resource and nw overhead
  4. Complex authentication and authorization scheme in the Microservices 

Design Considerations

  * **Cross-cutting**: microservices need not deal with details regarding problems outside their specific scope.
  * **Data sharing** is hard. Microservices tend to favor per-service or per-group databases that can be updated directly. 
  * **Availability**: Microservices, by virtue of being isolated and independent, need to be monitored to detect failures.
  * **Evolution**: Microservices tend to evolve fast. Old versions are usually available as long as there are clients who need to consume data from them. Newer versions are exposed in an application-specific way. For instance, with an HTTP/REST API, the version of the microservice may be part of a custom header, or be embedded in the returned data. Account for this.
  * **Automated deployment**: The whole reason that microservices are so convenient nowadays is that it is so easy to deploy a new service from a completely clean environment. 
  * **Interdependencies**: Keep them to a minimum. 
  * **Transport and data format**: Microservices are fit for any transport and data format; however, they are usually exposed publicly through a RESTful API over HTTP. Any data format fit for your information works. HTTP + JSON is very popular these days, but there is nothing stopping you from using protocol-buffers over AMQP, for instance.

microservices are developed almost in isolation. **Cross-cutting concerns** are dealt with by **upper layers** in the software stack