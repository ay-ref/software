# Software Engineering

- sbu course
- Dr. Mehran Alidoostnia

## s01

- solutions to big software problem
  1. virtualization
  2. containers
  3. less friction
  - serverless functions
  - edge computing

- software development firsts lifecycles
  - delivery pipeline
    1. build  
    2. test
    3. release  
  - feedback loop
    1. monitor
    2. planning

- devops = efficiencies that speed up software lifecycle

- development lifecycle
  - monolith
    - developers
    - one app
    - one build test release
  - microservice
    - teams
    - services
    - one build test release for each services

- old vs new
  - software
    - [ ] proprietary
    - [X] open source
  - scaling
    - [ ] vertical
    - [X] horiznotal
  - hardware
    - [ ] provisioning
    - [X] on demand infrastructure
  - testing
    - [ ] at the end
    - [X] as specs
  - release
    - [ ] periodic
    - [X] continuous delivery
  - architecture
    - [ ] monolith
    - [X] federated (microservice)
  - integrator
    - [ ] database
    - [X] api's
  - supervisor
    - [ ] product owners
    - [X] team leaders

- software development more modern lifecycle
  1. planning
  2. analysis
  3. design
  4. implementation
  5. testing and integration
  6. maintenance

## s02

- engineering
  - the use of scientific principles to build something
- software engineering
  - dealing with design, implementation, testing, maintenance
  of software application

- instructions
  - programs that execute desired function
- data structure
  - enable programs to adequately manipulate information
- descriptive information
  - describe program hard and virtual

- software application domains
  - system software
  - application software
  - engineering/scientific software
  - embedded software
  - product-line software
  - web/mobile applications
  - artificial intelligence

- legacy code
  - decades ago
  - meet changes for business requirement and computing platforms
  - proliferation causing headaches
  - costly to maintain
  - risky to evolve

- software engineering layers
  - tools
  - methods
  - process
  - a quality focus

- software process
  - activity
    - ex: communication with stakeholders
  - action
    - ex: architectural design
  - task
    - ex: conducting a unit test

- the process framework (5 activities)
  - communication
  - planning
  - modeling
  - construction
  - deployment

- umberlla activities
  - manage and control of
    - progress
    - risk
    - quality
    - change
  
- umbrella activities (8 items)
  - documentation
  - risk management
  - quality assurance
  - config management
  - reusablity
  - technical review
  - measurement
  - project tracking and control

- software engineering seven principles
  1. to provide value to its users
  2. kiss
  3. maintain the vision
  4. what you produce, others will consume
  5. be open to the future
  6. plan ahead for reuse
  7. clear and complete thought

## s03

- types of process flow
  1. linear
  2. iterative
  3. evolutionary
  4. parallel

- waterfall model of process
  - communication
    - project initiation
    - requirement gathering
  - planning
    - estimating
    - scheduling
    - tracking
  - modeling
    - analysis
    - design
  - construction
    - code  
    - test
  - deployment
    - delivery
    - support
    - feedback

- agility
  - pervasiveness of changes
  - team structure (communications)
  - continious delivery
  - customer as a part of dev team

- agile principles (12 items)
  - customer satisfaction
  - changing requirements
  - continous delivery
  - communicative regularly
  - support team member
  - face-to-face communication
  - measure work progress
  - development progress
  - good design
  - measure progress
  - continue seeking result
  - reflect and adjust regularly

- scrum
  - autonomous teams
  - product deliver incrementally
  - requirements may changes middle of the work
  - delivery devided into time-frames called sprint
  - roles
    - scrum master
    - product owner
    - development team members (up to 6 members)
  - artifacts
    - product backlog
      - prioritized list of functionality (to do list)
      - product owner is responsible
    - sprint backlog
    - code increments
    > back logs should be coherent with each others
  - events
    - sprint planning meeting
    - daily scrum meeting
    - sprint review meeting
    - sprint retrospective
  - burndown chart
    - x axis: time
    - y axis: story point (backlog)
    - one expected graph (ideal graph)
    - one actual graph
    - estimating the time
    - computing the velocity
  - velocity = work / sprint

- extreme programming (xp) framework
  - planning
    - user stories
    - values
    - acceptance test criteria
    - itration approach
  - design
    - simple design
    - prototypes
    - spike solution
    - crc cards
  - coding
    - refactoring
    - pair programming
  - testing
    - unit test
    - continuous integration
    - acceptance testing
  - release
    - incremental
    - computing project velocity

- kanban framework
  - properties (6 items)
    - visualize
    - limit work in progress
    - manage flow
    - explicit policies
    - feedback loop
    - improve/evolve

- lean framework
  - empower people
  - continuously improve
  - create value for the customer
  - eliminate waste
  - optimze value streams

## s04

- spotify model
  - tribe (alignment) (tribe lead)
  - chapter (functional area (specialist family)) (chapter leader)
  - squad (cross-functional autonomous team) (product owner)
  - guild (voluntary group to do some interests)

  - disadvantages
    - software sizing & cognitive load
    - heuristics for conway's law
    - patterns for team interactions
    - triggers for change and evolution

- cognitive load
  - the total amount of mental effort being used in the working memory
    - working memory: temporary memory for intermediate decision making

- cognitive load theory
  - intrinsic load
    - new information
  - germane load
    - linking new info to previous
  - extranaous load
    - unnecessary and distracting info

- conway's law
  - organizations which design systems are constrained
  to produce designs which are copies of the communication
  structure of these organizations.

- architecture of organization is more important than architecture of software.

- architecture
  - conway
    - your apps get shapes based on your organization
  - reverse conway
    - shape your organization based on app you want to make

- team first thinking
  - means of delivery
  - team cognitive load
  - boundaries for team ownership
  - physical and digital workspace

## s05

- requirement engineering
  - tasks and technique for understanding requirements
  - software engineering action
  - start from communication, end in modeling

- seven tasks of re
  1. inception
     - understanding problem, people who want solution, nature of solution
  2. elicitation
     - ask customers, users, and others to find product objectives
  3. elaboration
     - developing requirement model
  4. negotiation
     - resolving requirements conflicts
  5. specification
     - representation models
  6. validation
     - consistency
  7. management
     - change management

- uml diagrams
  - structrual
  - behavioral
    - activity
    - use case
    - state machine
      - simple
      - swimlane
    - interaction
      - sequence
      - communication
      - timing

- use case diagram
  - stylized story
  - end user pov
  - define actors

- activity diagram
  - choice, iteration, concurrency

- sequence diagram
  - process interactions over time
  - sequence of messages

- state diagram
  - states
  - events
  - [actions]

- initiative
  - epic
    - story/task
      - subtask

- user story
  - as a role, i feature, why

- good user story
  - independent
  - negotiable
  - valuable
  - estimable
  - small
  - testable

- scenario oriented acceptance criteria
  - given
  - when
  - then

- rule-based acceptance criteria

- srs
  - software requirement specs

- prd
  - product requirement document

## s06

- design classes
  - complete and sufficient
  - primitiveness
  - high cohesion
  - low coupling

- design model principles
  - design traceable to requirements
  - consider architecture
  - design of data is important as design of processing functions
  - interfaces should be design for its user
  - component-level design should be functionally independent
  - components should be loosely coupled
  - design should be understandable
  - design developed iteratively
  - not preclude agile approach

- c4 model
  - context diagram
    - our system communication with external available systems and customers
  - container diagram
    - zoom to our system, showing our system services apps
  - component diagram
    - zoom to our services, showing main functionality of our services
  - code diagram
    - zoom to components, showing classes of code

- architectural style
  - data-centered
  - data-flow
  - call-and-return
  - object oriented
  - layered
  - multitier

- layered example: mvc
  - model, view, controller
    - view ---sees---> user ---uses---> controller
    ---manipulates---> model ---updates---> view

- modern architectural style
  - monolith
  - soa (service oriented architecture)
  - asynchronous messaging
  - ddd (domain-driven design)

- monolith
  - unified-unit
  - self-contained
  - independent from other applications
  - small
  - lack of flexibility
  - difficult to scale

- soa
  - services
  - each service provides business capability
  - services communicates with each other across platform and languages
  - esb
    - enterprise service bus

- microservices
  - small independent services
  - services communicates with apis
  - each service one small, self-contained team

- microservices vs soa
  - architecture
    - ms: design to host services that function independently
    - soa: design to share resources across services
  - component sharing
    - ms: does not involve sharing
    - soa: frequently does sharing
  - granularity
    - ms: fine-grained
    - soa: coarse-grained
  - data storage
    - ms: each service can have independent storage
    - soa: involve sharing storage between services
  - governance
    - ms: require collaboration between teams
    - soa: common governance protocols between teams
  - size and scope:
    - ms: smaller and web-based application
    - soa: large scale integrations
  - communication
    - ms: apis
    - soa: esb
  - coupling and cohesion
    - ms: bounded context for coupling
    - soa: sharing resources
  - remote services
    - ms: rest and jms
    - soa: soap and amqp
  - deployment
    - ms: quick and easy
    - soa: less flexible

- communication
  - synchronous
    - real-time
  - asynchronous
    - without real-time conversation
    - multiple services
    - allow failure and retry
    - take a lot of time

- synchronous communication
  - rest
  - grpc
  - graphql

- rest
  - over http protocol
  - json payload and response
  - serilization and deserialization
  - hard to adhere all principles

- grpc
  - google remote procedure call framework
  - high performance
  - connecting microservices

- graphql
  - open-source data query langague
  - excelent developer experience

- asynchronous communication
  - rabbitmq

- domain driven design
  - you should have a ubiquitous language

## s07 - ddd

- domain
  - about
    - knowledge
    - influence
    - activity
  - the subject area to which the user applies a program

- ddd
  - domain driven design
  - a software design method wherein developers construct
  models to understand the business requirements of a domain.
  - these models serve as conceptual foundation for developing
  software.
  - approach for building complex software applications that is
  centered on the development of an object-oriented domain model.

- the most important subject in DDD is
  - ubiquitous language
    - a common language between all model related objects!
      - subject
        - developer
        - domain expert
        - business analyst
      - object
        - planning sessions
        - code
        - documentation
        - specs & requirements
    - contains
      - domain model terms
      - ddd paterns
      - bounded contexts
    - connectors of
      - technical terms, concepts, aspects, design patterns
      - business model, business terms, business of business

- advantages
  - simple communication
  - more flexibility
  - the domain is more important than ui/ux
- difficulties
  - deep domain knowledge is needed
  - contains repetitive practices

- ddd patterns
  - strategic
    - analyze domain
    - define bounded contexts
    - identify microservices
  - tactical
    - design individual services

- strategic
  - bounded context (bc)
    - business concepts(sometimes policies) like security, ...
    - space in which a term has
      - definite
      - unambiguous meaning
    - problems
      - false cognates
      - duplicate concepts
    - partitions of subdomain
  - context map
    - relationships between bcs
  - domain
    - one partition of model
  - sub-domain
    - one partition of domain
    - each maps to a service
    - one expert for each
  - ubiquitous language
  - ci
  - domain model

- tactical
  - value objects
    - importance is value
    - contains
      - data
      - behaviour
    - always immutable
    - patterns
      - essence
      - builder
  - entities
    - importance is identity
    - contains
      - data
      - behaviour
    - every entity has a unique id forever
    - always mutable
    - does not mean every property of entity should/can change
  - aggregate
    - connects each other by domain events
    - group of entities and value objects with certain characterestics
      - it is behave as a whole in
        - creatoin
        - retrieving
        - storing
      - always in consistent state
      - it owned by an entity called the aggregate root
    - aggregate constraints
      - can be referenced only from outside by every entities just
      through its root
      - granularity trade of between
        - consistency
        - scalability
  - layers
    - infra
    - adapter
      - otehr layers connector
    - application
    - domain
      - whole logic of ddd is here
  - repositories
  - services
  - factories
  - modules

- three steps of microservice architecture
  - identify system operations
  - identify services
  - define service apis and collaborations
  
- microservice
  - monolith first
  - microservices first
    - ddd required!!!

- right size of microservice architecture
  - aggregate <= microservices <= bounded contexts

## s08 - netflix architecture

- open connect (oc)
  - netflix custom global cdn
  - advantages
    - less expensive
    - better quality
    - more scalable

- amazon aws
  - amazon s3
    - simple storage service
  - amazon ec2
    - elastic compute cloud

- react advantages
  - starup speed
  - runtime performance
  - modularity

- elb
  - elastic load balancer
  - traffic routing
  - two-tier
    - zones first
    - instances then

- zuul
  - gateway service
  - easy routing
  - inbound filter
    - authentication
    - routing
    - decorating
    - route to endpiont filter
  - netty server
    - network protocol
    - proxying work
    - connection management
  - endpoint filter
    - returns static response
    - forward request to backend
    - once request recieved from backend forward to outbound filter
  - advantage
    - create rules and share
    - load testing
    - test new services
    - redirection

- critical microservices
  - dependent and independent to some specific services
  - dependent just on reliable services

- evcache
  - data frequently used
  - faster response
  - custom caching layer

- databases
  - mysql
  - cassandra

- mysql
  - acid
  - master-master

- cassandra
  - large data
  - more users
  - more history
  - smaller storage footprint
  - consistent read write speed

- sql vs nosql
  - highly structured vs unstractured
  - transaction oriented vs flexibility schema
  - data integrity & security vs horizontally scalable
  - complex queries vs no overhead for structure

- kafka
  - higher volume and velocity
  - thousands of messages per second

- elasticsearch
  - distributed search and analytics engine
  - clusters
  - hosts

- spark
  - analytics engine
  - machine learning
  - content recommendation

## s09 - rest api

- web api should support
  - platform independence
  - service evolution
    - independent from clinet applications
    - api evolves client applications function without modificaiton

- api design lifecycle
  - requirement engineering
  - api design
  - api review
  - implementation
  - user testing
  - release
  - deprecate

- requirement engineering
  - collect data with pair programming
  - user experience research
  - exposure hours
  (total number of hours worked by all employees within a calendar month.)

- api releases
  - postman collections
  - mock servers
  - sdk's
  - documentation

- api releases
  - beta
  - gated features
    - continous monitoring on released features & selected features

- rest api
  - rest (representational state transfer)
  - architectural style
  - rest is independent of any underlying protocol
  - design principles
    - designed for clients around resources
      - object
      - data
      - service
    - a resource has an id
    - clients interacts by exchanging representations of resources.
    - json as exchange format
    - decouple client & service
    - stateless request model

- rest api over http
  - http verbs
    - get
    - post
    - delete
    - put
    - patch

- best practices
  - naming
    - uri's based on nouns
    - avoid jargons
  - collections
    - collections have their own api's
    - using plural noun for colllections
    - routing to the item in the collection with id after
    uri of collections
  - associations
    - showing relationsihp between resources in uri's
  - filter
    - should define for best usage
    - includes in query of uri (usually after `?`)
  - pagination
    - data in collections can be very large
    - so we should limit the data returned from the request
  - sort and fields
    - similar strategy of filtering just for sort based on what
    - similar strategy of filtering just showing fields specified
  - using asynchrounous operations
    - returning current status of request processing before
    sending the response

## s10 - ci/cd

- ci (continous integration)
  - integerating all your code changes into the main branch
  of a shared source code repository early and often automatically
  testing each change when you commit and automatically kicking off
  a build.
  - errors and security issues can be identified and fixed more
  easily and much earlier.

- cd (continous delivery)
  - software development practice that works in conjunction
  with ci to automate the infrastructure provisioning and
  application release process.
  - deployed to production at any time.

- ci/cd overview
  - plan
  - ci
    - code
    - build
    - test
  - cd
    - test
    - release
    - deploy
  - operate

- ci/cd fundamentals
  - single source repository
  - frequent check-ins to main branch
  - automated builds
  - self-testing builds
  - frequent iterations
  - stable testing environemnt
  - maximum visibility
  - predictable deployment anytime

- staging environemnt
  - complex software is hard to test
  - deploy a complete production-like environment,
  but don't have everyone use it
  - lower risk if problem occurs in staging that in production

- environment (for testing)
  - developer environment
  - staging environment
  - production environment

- operations responsibility (devops)
  - once we deploy someone has to monitor software
  , make sure running ok, no bug

- monitoring
  - hardware
    - voltage
    - temperature
    - fan speeds
    - component heaalth
  - os
    - memory usage
    - swap usage
    - disk space
    - cpu load
  - middleware
    - memory
    - thread/db connection pools
    - connections
    - response time
  - applications
    - business transactions
    - conversion rate
    - status of 3rd party component
  - ex: elk stack
    - elastic search
    - logstash
    - kibana

## s11 - ux

- ux (user experience)
  - defines the experience of a user in the company,
  its services and its products environment.

- ui (user interface) elements
  - colors
  - typography
  - content layout
  - buttons and icons
  - menus
  - forms
  - images

- ux key components
  - user research
  - information architecture
  - visual hierarchy
  - wireframing
  - user flows and personas
  - prototyping
  - iterative testing and feedback
  - accessibility

- ux research
  - understanding how customers interact with your brand
  - how easily they can complete their tasks and meet their goals

- information architecture
  - users
  - content
  - context

- ux metrics
  - bounce rate
  (the percentage of users who arrive at your site, but don't come in.)
  - events (scrolling, first visit, menu click, file download)
  - new users
  - page views
  - user engagement
  - view per user
  - user retention
  - churn rate
    - chrn rate = (customersT0 - customersT1) / customersT0

- design thinking
  - problem solving
  - innovation
  - aplly on desciplines and industries
  - strong emphasis on understanding the needs
  and perspectives of users or customers
  - creative & effective solution

- design sprint
  - 5-day process
  - user-centered teams tackle with design problems
  - expert insights
  - team ideate
  - prototype
  - test solutions
  - selected users
  - 5 phases
    - understand
    - sketch
    - decide
    - prototype
    - validate

## s12 - design patterns

- design patterns
  - standard solution to a standard problem in a context
  - abstract from programming languages
  - identifies classes and their roles in the solution

- benefits of design patterns
  - common vocabulary
    - abstract the problem
    - increase design speed
  - expertise communication
    - design reuse, avoid mistakes
    - system is easy understandable
  - improve documentation
    - improve understandablity

- gang of four (gof) patterns
  - creational
    - factory method
    - abstract factory
    - singleton
    - builder
    - prototype
  - structural
    - adapter
    - bridge
    - composite
    - decorator
    - facade
    - flyweight
    - proxy
  - behavioural
    - command interperter
    - iterator
    - observer
    - mediator
    - state
    - strategy
    - chain of responsibility
    - visitor
    - template method

- describe a pattern
  - problem
    - situations
  - solution
    - what is the pattern?
  - pros and cons
    - advantages
      - why the pattern is useful?
    - disadvantages
      - why someone not want this pattern?

- acid
  - automicity
  - consistency
  - isolation
  - durability

- design pattern: saga
  - problem
    - how to implement transactions that span multiple services?
  - solution
    - each transaction with span multiple services called saga
    - a saga is a sequence of local transactions
    - each transaction updates the database and publish message
    - if a local transaction fails, do compensating(undo) transactions
    - 2 ways of coordination
      - choreography
        - each local transation publishes domain events
        that trigger local transactoins in other services
      - orchestration
        - an orchestrator tells the participants what local
        transactions to execute
  - advantages
    - it enables application to maintain data consistency
    in distributed transaction
  - disadvantages
    - the programming model is more complex ex: designing undo transactions

- design pattern: cqrs
  - problem
    - a query that retrieves data from multiple services in microservice
  - solution
    - define a view database which is read-only replica to support the query
    - keep the replica up to date by subscribing domain events

- design pattern: factory
  - problem
    - creating object without to specify their exact class
  - solution
    - creating object by factory method instead of constructor
    - define a factory method within the superclass that defers
    the object creation to subclass factory method

- design pattern: adapter
  - problem
    - reuse from a class without interface
    - working incompatible interfaces together
    - alternative interface for a class
  - solution
    - define a seperate adaptor class that complete
    our incompatible interface(s)

- design pattern: strategy
  - problem
    - we need select algorithm at runtime
  - solution
    - instead of implementing single algorithm directly
    implement an strategy(operator) class that some algorithms
    inherits from it and use from operator method in your main class
