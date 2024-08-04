# System Design

## Computer Architecture

- units of data
  - bit
  - byte(ex: 1, A) = 8 bits
  - KB = 1000 bytes
  - MB = 1000 KBs
  - GB = 1000 MBs
  - TB = 1000 GBs

- data at last of it's path stored in disk storages

- disk storage
  - non-volatile (keep save without power)
  - all of os, files, ... save here
  - types
    - hdd
    - ssd
  - range
    - 128GB ... 2TB

- hdd vs ssd
  - speed
    - hdd: 80 MB/s - 160 MB/s
    - ssd: 500 MB/s - 3,500 MB/s

- after disk we have ram for data access

- ram
  - volatile (power required)
  - all of app runtime data like data structures, variables, ... stored here
  - size range
    - 2GB - 128GB
  - access time
    - microseconds

- next data access is cache

- cache
  - volatile (power required)
  - all of most probability time usage data stored like registers
  - range
    - MBs
  - access time
    - nanoseconds

- cache is ususally besides of cpu

- cpu
  - runs the codes
  - high-level codes translate to machine-level code (binary)
  - cpu do read/write on disk, ram and cache

- motherboard
  - board that everything is on it and have connection for relate them

## High-Level Software Architecture

- ci/cd
  - continous integration / continous deployment
  - series of tests and pipeline checks
  - deployment
  - examples
    - jenkins
    - github actions

- load balancer
  - solution of many users that does high load on server
  - example
    - nginx

- server application is the code runned on main servers
  - this can talk to many external services

- we need some additional server next to main servers for storage

- to ensure everything is running smoothly we need logging and monitoring system
  - we monitor logs
  - analyze them
  - backend example
    - pm2
  - frontend example
    - sentry

- also we have an alert system
  - when some important event happened it notifies the target
  - in modern architecture it is integrated to slack

- for finding and repairing the bug you should debug on the staging not production

## Pillars of Good Design

- good design
  - scalability
    - system can grow
  - maintainability
    - developers can communicate with design
  - efficiency
    - best use of resources
  - reliability
    - handling failure as good as possible

- 3 key actions with data
  - moving data
    - between servers, client-server, databases
  - storing data
    - sql, nosql
    - access patterns
    - indexing strategies
    - backup solutions
  - transforing data
    - converting data to meaningful information

- cap theorem (brewer's theorem)
  - a design at the best can have 2 of 3 below!:
    - consistency
      - all nodes have same data at the same time
    - availability
      - always server is up despite everything happens behind the scenes
    - partition tolerance
      - when one partition is out others do works fine
  - examples
    - cp (consitency-partition tolerance)
      - banking system: ex: when some transaction needs more time for secure transferring

- we cannot find perfect solution
we find the best solution for our specific situation

- availability
  - has a percentage meter
  - ex: 99.9 % means 8.76 hours of downtime per year permitted
  - ex: 99.999 % means 5 minutes of downtime per year permitted
  - 2 contract
    - SLO: Service Level Objects
    - SLA: Service Level Agreements

- reliability
  - system works correctly and consistently

- redundancy
  - having backup ensuring that when one node is down it can replaced

- speed
  - throughput
    - how much data our sever can handle over a certain period of time
    - server throughput - rps = request per second
    - db throughput - qps = query per second
    - data throughput - bps = byte per second
  - latency
    - how long to handle a single request

## Networking Basics

- ip address
  - unique identifier for each node (computer)
  - types
    - ipv4
      - 32 bit
      - 4 billions address
    - ipv6
      - 128 bit
      - 340 trillions address

- packet
  - ip header
    - senders ip
    - receiver ip
  - internet protocl (ip)

- application layer
  - http protocl

- transport layer
  - tcp
    - reliable communication
    - tcp header
    - 3way handshake (syn, synack, ack)
  - udp
    - unreliable communication
    - faster communication
    - good for video call, streaming, ...
    - data loss is acceptable

- dns
  - domain name system
  - maps domain name to ipv4 address
  - icann
    - internet corporatoin for assigned names and numbers
    - domain name distributor

- network insfrastructure
  - pulic ip address (for public internet)
  - private ip address (for lan)

- ip address
  - static
  - daynamic

- for managing communication to the lan we use firewall
  - monitoring
  - controlling

- ports are where data goes in and goes out
  - http: 80
  - https: 443
  - ssh: 22
  - mysql: 3306

### Application Layer Protocols

- http
  - hypertext transform protocol
  - built on tcp/ip
  - stateless conversation
  - requests includes all neccessary information
  - status code
    - 2xx - success
      - 200 - ok
      - 201 - created
      - 204 - no content
    - 3xx - redirection
      - 301 - move permanently
      - 302 - found
      - 304 - not modified: use from cache!
    - 4xx - client error
      - 400 - bad request
      - 401 - unauthorized access
      - 403 - forbidden
      - 404 - not found
      - 429 - too many request: based on rate limiting

- http is one-way connection, for real time connection we use
websockets that have 2 way real time channel we have no request response cycles

- email relative protocls
  - smtp
  - imap
  - pop3

- file sharing
  - ftp
  - ssh

- real time communication
  - webrtc
  - mqtt
  - amqp

- rpc
  - invoke a function in another computer
  - ex: http or smtp make a function call at backend server

## API Design

- crud operations
  - create: post /api/products
  - read: get /api/products
  - update: put /api/products/:id
  - delete: delete /api/products/:id

> usually used in http but same paradigm on grpc and graphql

- communication protocl
  - http
  - websocket

- data transport format
  - json
  - xml

- api paradigms
  - rest
    - stateless
    - http
    - over-fetching/under-fetching
    - json format
  - graphql
    - avoid over-fetching/under-fetching
    - strongly typed schema based queries
    - queries can impact server performance
    - only post request
  - grpc
    - built on http/2
    - multiplexing / server push
    - uses protocol buffers
    - less human readable
    - http/2 is required

- api should have rate limiter for ddos attack defending
- api should use from cors to manage which domain can access your api

- for solving the latency in long geographical distance
we use from cdn (content delivery network) and caching technique

- cache
  - hit
  - miss
  - cache ratio = (hits) / (hits + miss)

- caching
  - browser
    - requests checks to cache
  - server
    - requests goes to cache
    - redis server
    - memcache server
  - database
    - queries goes to cache
  - cdn
    - networks of servers
    - types
      - pull-based
      - push-based

- write to cache
  - write around
    - write to db and cache by server same time
  - write back
    - write to cache then cache write to db
    - loss data possible

- cache should use from eviction policies
  - common is lru (least recently used)
  - or fifo
  - or lfu (least frequently used)

- cdn benefits
  - reduced latency
  - high availability
  - improved security

- proxy server
  - a server between client and main servers
  - pupose
    - caching resources
    - anonymizing requests
    - load balancing
  - types
    - forward proxy
    - reverse proxy
    - open proxy
    - transparent proxy
    - anonymous proxy
    - distorting proxy
    - high anonymity proxy

- load balancer algorithms
  - round robin
  - least connectoin
  - least response time
  - client ip hashing
  - geographical algorithms
  - consistenting hashing
  - all algorithms can be used in weighted way

- load balancer should have health check for finding
healthy severs

- load balancer examples
  - software
    - nginx
    - haproxy
  - hardware
    - citrix
    - f5
  - cloud-based
    - aws
    - google load blanacer

- for solving the single point of failure of load balancer we
use from extra load balancer server and partitoin clients between servers

- with dns fialover we can change the dns of unhealthy loadbalancer to a healthy
load balancer

## Database

### Relational Databases

- examples
  - postgres
  - mysql
  - sqlite

- sql
  - structured query language

- features
  - greate for transactions
  - complex queries
  - integrity

- acid compilant
  - atomicity
  - consistency
  - isolation
  - durability

### NoSQL Databases

- ACID without C (consistency)
- examples
  - mongodb
  - casandra
  - redis

- redis
  - key-value-based

- mongodb
  - document-based

- neo4j
  - graph-based

- features
  - scalibitliy
  - quick iteration
  - simple queries

- in-memory databases
  - redis
  - mem-cache

### Scaling Databases

- vertical scale up
  - increase cpu power
  - adding more ram
  - adding more disk storage
  - upgrading network

- horizontal scale out
  - sharding
  - replication

- sharding strategies
  - range-based
  - directory-based
  - geographical

- replication
  - master-slave
  - master-master

### Database Performance

- caching
- indexing
- query optimization
