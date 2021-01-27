# Cloudy Thursday ep. 2 
###### tags: `show`


## Introduction

> Every episode have to have this one the same, we do forget about it.

> Hello and welcome to cloudy thursday, your weekly dose of cloudy news from around the interwebs.
> I am Petr Kotas and I am one of your hosts tonight.
> I am Robert Zahradnicek and I am your next host for tonight.
> Just a reminder, eveything we say here is our, and ours only. It does not represent our employer.
> Today's guest is Peter Malina, a Google Developer Expert and a CTO of FlowUp. Peter's here to talk with us about Monoliths, Microservices, and their resiliency

- Who we are
- How have we been
- Something interesting we are working on / anything really
- Disclaimer everything we say is our opinion
- Repeat the topic what are we going to discuss


## Topic

> The topic for discussion on this episode

Application resilience and development.


## News 

> Was there anything interesting


## Discussion notes

> To refresh our memory on the go

- @petomalina 
    - The talk about Microservices vs Monoliths is not about technology, but people (and wherever people are, failures are)
    - Everything we engineer is bound to break in the future
    - The biggest failure of systems I engineer is future me
    - How do we know we can recover, when we never failed? Shoulf we fail proactively to make sure we don't fall too hard?
    - Make our own disasters (shut down the system, delete the database, don't let the main maintainer intervene in a fake incident, etc.)
    - Microservices are meant for resiliency against us (team). If there's no team, there's no new need for new microservice
    - Composable microservices (isolated "modules", that can be deployed as a monolith as well as a microservice cluster)
    - Learning Curve vs Value Curve of a technology
    - Supply chain of services - know your dependencies
