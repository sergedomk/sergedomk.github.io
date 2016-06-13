class: center, middle
# Micro-services provide some benefits, but at what cost?
## Serge Domkowski <sdomkowski@kavi.com>
.footnote-center[Presentation created using remarkjs http://remarkjs.com/]
---
## Who am I?

__Serge Domkowski__ .red[*]  
_Software Architect_

I’ve been involved in making web software for about 22 years. I design and
write code, talk about code, play with my son, ride my bicycle, root for the
Timbers, drink beer, and once in a while sleep.

__Kavi Corporation__ .red[**]   

_Our mission is to help results-driven teams share and organize complex work._

- 22 Employees
- 8 Engineers

.footnote[
  .red[*] <sdomkowski@kavi.com>

  .red[**] http://www.kavi.com
]
---
class: center, middle
# Why am I here?
## To discuss some hard choices concerning micro-services.
---
class: center, middle
# Why Micro-services?
## Specifically, What Were Our Objectives?
---
## Scalability

Customer size and resource utilization varies drastically. Customer bandwidth
requirements tend to be low to moderate with spikes during the calendar year.
Some application features/components are utilized far more than others.
---
## Scalability

Customer size and resource utilization varies drastically. Customer bandwidth
requirements tend to be low to moderate with spikes during the calendar year.
.red[__Some application features/components are utilized far more than others.__]

.center[
## Micro-services would allow us to scale<br>specific business components independent<br>of other business components.
]
---
## Flexibility

Customer requirements are evolving as new technologies arise. This results in
the need to be able to integrate these new technologies into or with our
application and the need for our existing functionality being adaptable to
the future needs of our customers.
---
## Flexibility

Customer requirements are evolving as new technologies arise. This results in
the need to be able to integrate these new technologies into or with our
application and the need for our existing functionality being adaptable to
the future needs of our customers.

.center[
## Interfaces represent business logic which tend<br>to be easy to adapt to external services.
]
---
## Maintainability

Advances in technology, new security concerns, and evolving customer needs
require rapid development. We expect that 50-80% of the code today will be
obsolete in 5 years. The application must be able to handle changes without
degrading quality.
---
## Maintainability

Advances in technology, new security concerns, and evolving customer needs
require rapid development. We expect that 50-80% of the code today will be
obsolete in 5 years. The application must be able to handle changes without
degrading quality.

.center[
## Micro-services can be replaced at will!
]
---
class: center, middle
# What could possibly go wrong?
## And how do we deal with it?
---
class: center, middle
# #1.
## Misjudged the complexity.
---
## Asyncronous Communication

--

* __Order of Operations__
--

  * Requeuing
--

* __Failures / Timeouts__
--

  * Dead Letter Queue
  * Monitoring
  * Tracebacks
--

* __Latency__
--

  * Forced Lag
  * Re-checking
  * Obscurity
  * Notification
--

* __Debugging__
--

  * Configurable Logging
  * Log Analytics
  * QA Cluster
---
## Inter-service Dependencies
--

* __Planning__
--

  * Establish Usage Patterns
  * Determine Suitable Services
  * Architectural vs. UX Documentation
--

* __Deployment__
--

  * API Versioning
  * Pre-deployment of Dependencies
--

* __Duplication__
--

  * Code Libraries
  * Replication of Data
---
## Interfaces, Interfaces, Interfaces.

--

* __Documentation__
--

  * Automated Code Documentation
  * Automated API Documentation
  * Architectural Documentation
--

* __The Tangled Web__
--

  * Limited Depth
  * Established Usage Patterns
  * Topic Exchange
---
class: center, middle
# #2.
## Forgot to ask the customer what they needed.
---
## Process Control
--

* __Service level Configurability__
--

  * Stored Service Configuration/Customer
--

* __User level Configurability__
--

  * Stored Client-Side Configuration/Session
---
## Activity Reporting
--

* __Data Replication__
--

  * Duplication of Data
  * Aggregation of Data
---
class: center, middle
# How has this changed what we do?
---
## Product/UX/Architecture Three Month Plan
--

## REST can not solve everything
--

## Duplication is not evil
--

## Error handling is critical
---
class: center, middle
# Questions?
---
## Further Reading

__AMQP 0.9.1 - Advanced Message Queuing Protocol__
http://www.amqp.org/specification/0-9-1/amqp-org-download

__Microservices - a definition of this new architectural term__
http://martinfowler.com/articles/microservices.html

__Service Oriented Architecture__
http://www.opengroup.org/soa/source-book/soa/soa.htm

__No Silver Bullet - Essance and Accident in Software Engineering__
http://worrydream.com/refs/Brooks-NoSilverBullet.pdf

__Dependency Oriented Thinking - Volume 1__
https://www.infoq.com/minibooks/dependency-oriented-thinking-1

__Dependency Oriented Thinking - Volume 2__
https://www.infoq.com/minibooks/dependency-oriented-thinking-2

__Flow Based Programming__
http://www.jpaulmorrison.com/fbp/

