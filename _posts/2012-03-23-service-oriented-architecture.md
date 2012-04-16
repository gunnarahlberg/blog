---
layout: post
title: From vendor lockin to service oriented architecture
    
---

{{ page.title }}
================

<p class="meta">Published {{ page.date | date : "%Y-%m-%d" }}</span> - Stockholm</p>
To replace a custom system written on top of a vendor platform to a system without lock-in, avoid the silos and build structures that reflect your business values.
<img src="/images/uploads/2012/04/silos.jpg" alt="Silos" />
    
First steps
-----------
First, define a subsystem that is self contained. Develop that system and deploy to production as soon as the new subsystem can replace functionality in the old system. Continue to move subsystems to the new platform and eventually, the old system can be shut down. This strategy is called strangling or starvation.

Frameworks and accidental complexity
------------------------------------
To use a standard platform may, but not necessarily, end up in a system driven by the standard of the platform rather than the value adding services of a company. When I've used Polopoly, the system was a defined in subsystems by the Polopoly framework rather than by the business. The code base was tangled with cross references and dependencies that hampered one business unit from another. Let the organisation of the IT-system be a mirror of the business organisation. This yields a system with less accidental complexity.

Define Subsystems 
-----------------
If the client has an application that is hard to maintain due to accidental complexity it is good idea to define separate subsystems that in themselves add business value. To coordinate the subsystems, a variety of techniques of well high quality are available, such as Enterprise Service Bus, Point-to-Point, RMI, SOAP and WSDL or RESTful services. Technology is irrelevant, it is added business value that matters, adapt to change and understanding that applications are developed by people. That matters.

Team structure and architecture
A system owner, architect or developer will often get a system that is a reflection of the organisation structure of the development. If all developers are part of the same team, the code will quickly become a coherent complex of parts. If the structure is divided in teams and each team is responsible for one or two business services, the IT-system quickly becomes subsystems that have specific business value. The benefits of this structure is that architectural and privatization becomes easier. What happens is that the subsystems can be prioritised based on business value.

IT-systems based on business services
-------------------------------------
Amazon. For Amazon it is important to be able to scale. Both in the number of developers, testers, business analysts, systems, data demand and data bandwidth and that those scalability decisions is defined from the business value. The Amazon answer is that each team is cross-functional, with business analysts, developers, testers and maintenance in one team. The call this "two pizza teams" - that's the number of people that can share two pizzas. <http://highscalability.com/amazon-architecture>

Technologies
------------
The technologies that can be used are a number, my favourite is the strategy described by Jim Webber and Martin Fowler in the presentation "Does my Bus [Enterprise Service Bus] look big in this?" <http://www.infoq.com/presentations/soa-without-esb> - a funny and interesting 45 minute presentation, lot's of fun!
The gist of it is that, define your integrations not on a framework or library or platform defined by the middle-ware vendors but rather by a set of techniques that have been around for a long time. Skip forward to minute 30 of that presentation were Martin Fowler describes traditional SOA compared to guerrilla SOA. Same set of promises of orchestration, contracts, information model definitions yet without the complexity and vendor lock-in.

Suggestion
----------
Chose integration strategy based on simple standard technologies that have been around for a long time. Use specific tools that are good at one or two things and combine them together. Incidentally, this is what Unix so good.

