# SDET interview questions

## Purpose
The purpose of the interview is to determine level of hard and soft skills and to check
that person fits team mentally.

## Approach
- prefer open questions: ie. questions without one correct answer.
- when asking binary questions, mix yes and no questions. Don't coerce everything into yes or no.
- ask not only about **what**, but also about **when** and **why** explanations.

## Structure
- greeting and small-talk
- project introduction
- soft skills (past experience, English level, etc.)
- hard skills
- Q&A

## Soft skills
- Role on previous project (what was doing, team size, what learned, etc)
- How frequently was your product released? Your involvement in the releases?
- Development methodology (Scrum, Kanban, Warefrall). When to use what?
- QA process (code review, code intelligence, CI/CD)
- Good/bad practices
- Ideal QA/delivery process (Jira, VCS, CI/CD)
- Notable tools

## Theory

### General QA
- Testing pyramid
- Test documentation
- Functional vs integration vs e2e tests
- What's easier to test: monolithic application or microservices?
- Who should be responsible for quality?
- Who should test?
- When should automation start?
- Shift left/right

### Test design
- Provide test cases for application with an input field that accepts 0 - 10 numbers (inclusive). Decimals are allowed and will be rounded to the whole number using mathematical rounding. Application saves Integer in the DB.

### Computer science
- OOP (4 principles, basic use cases)
- Design Patterns
- Anti-patterns
- Clean code (SOLID, GRASP, DRY, YAGNI)
- Algorithms (Big O notation, basic algorithms)
- Multiple inheritance
- Composition/aggregation vs inheritance
- Method vs function

### General QA automation
- Test framework design/architecture (basic approaches, organization, must-use patterns)
- Metrics: limiting test run time and resource utilization/test run optimization
- Configs
- Data preparation and cleaning
- Logs
- Reporting
- CI integration
- Tool integration

### Java
- primitives/objects
- mutable/immutable
- var (if Java 11)
- interfaces vs abstract classes
- annotations
- override/overload
- collections
- list/set/map
- hash map/hash set
- stream
- lambdas
- optional
- generics
- equals and hashCode
- deep clone/shallow clone
- exceptions (checked/unchecked/errors)
- try/catch/finally
- static (method, variable)
- final (class, method, variable)
- access modifiers (default for class, interface)
- constructor/initializer
- JMM (heap/stack, garbage collectors, happens before, reordering, JIT)
- multithreading (asynchronous execution, reactor, locks, synchronization, thread pool, executor service, future)
- jUnit/TestNG/... (testability, mock vs stub vs spy, annotations, configuration, parallel run, parametrization)
- Maven/Gradle/... (role, configuration, dependencies, plugins, phases)

### Python
- code style/quality (PEP8 / PEP20)
- mutable/immutable data types
- constructors (how to implement?)
- tuple vs list vs set
- list/dict comprehension
- the difference between v2 and v3
- is vs ==
- lambdas
- generators vs iterators
- dict
- decorators
- magic methods
- type hints
- arguments (*args, **kwargs)
- global/nonlocal
- is Python interpreted or compiled
- slicing (list, str)
- how to reverse iterable object
- try/catch/finally
- keyword **pass**
- keyword **with** (context manager)
- keyword **yield**
- copy/deepcopy
- keywords break/continue/pass
- venv/pipenv
- _var and __var (protected vs private)
- multithreading/asynchronous code
- GIL

### Spring Boot
- The main idea behind Spring (IoC, Proxy)
- Differences between Spring (MVC) and Spring Boot
- Main annotations and their roles
- Bean scopes (default bean scope)
- Bean cyclic dependency

### Hibernate
- JDBC/Hibernate/Spring Data
- Entity
- Entity relations
- N+1 problem

### pyTest
- fixtures
- fixture scopes
- parallelism
- hooks
- parametrization
- marks

### Selenium
- page object
- waits (interaction between implicit and explicit during waiting for object to disappear)
- remote driver
- selectors
- findElement/findElements return type in case of failure
- StaleElementException
- On what part of element will Selenium click?
- Element not clickable at point
- Download/upload file
- JS executor
- Actions
- basic auth (http)
- avoid login in every new test
- Parametrized locator
- DOM

### XPath
- Differences / and //
- Differences . and ..
- Wildcard *
- Keyword contains
- Search by text
- Get parent element

### REST
- relation to HTTP
- methods
- differences between GET and POST
- differences between PUT and POST
- PATCH, HEAD, OPTIONS
- idempotency
- query string (what is used for, limitations)
- components (verb, header, body, etc)
- supported markup languages
- status codes
- streaming (WebSockets / HTTP2)

### Microservices
- SOA vs DDD
- REST
- gRPC/Protobuf
- Kubernetes
- Docker
- Service discovery
- Cloud-agnostic tools
- Graceful degradation
- Circuit breaker
- Saga

### Git
- fetch vs pull
- merge vs rebase
- merge conflict
- force-push (what --force-with-lease does?)
- revert commit
- squash
- stash
- reset (—mixed, --hard, --soft)
- merge —abort
- fork

### SQL
- SQL/noSQL
- noSQL DB types (key-value, document-oriented, wide-column, time series)
- basic syntax
- joins
- subqueries
- group by / having
- distinct
- union
- indexes
- transactions (isolation levels)
- normalization
- Transaction isolation level
- CAP theorem
- ACID

### Docker
- container vs image
- networking (network types, ports, discovery)
- containerization vs virtualization
- Dockerfile: FROM, ADD, COPY, RUN, CMD, ENTRYPOINT
- docker pull/info/stats/images
- latest tag
- data persistency (volumes, mounts, permissions)
- compose
- swarm

### Networking
- address vs netmask
- ISO/OSI
- bridging vs routing vs switching
- protocols (tcp, udp, icmp)
- routing (BGP, OSPF)
- DHCP
- ARP
- VPN and VLAN
- packet anatomy

### Jenkins
- Jobs
- Pipelines
- Jenkinsfile
- Built-in environment variables
- Useful plugins

### Linux
- logs
- change permissions
- open file (read/update)
- create/rename/remove/copy file
- default env variable value :-
- stop process
- find file

### Cloud
- cloud native technology benefits
- lift and shift issues
- cloud issues
- IaaC (Cloud Formation, Terraform, Pulumi)
- Serverless

### Leadership
- Conflicts inside the team
- Project estimation
- Team velocity and performance
- Firing people
- What to do if a team member refuses to work?
- Team stabilization/working with attrition and demotivation/burnout

### Extra
- Mock vs stub vs spy
- Wiremock / MockServer and similar (mock TCP server)
- BDD (example of BDD test, when to use / not use)
- JSON / XML
- CI/CD (Jenkins/GitLab, integration, jobs, pipelines)
- GitHub actions
- Linux (command line, ssh, find/locate, pipes, editors, resource monitoring, logs, access rights)
- NoSQL (time-series DBs, keys, nesting, hot keys, deduplication, normalization)
- Message queues (RabbitMQ, Kafka, concepts, delivery guarantee)
- VCS (Git, Mercurial) (branches, pull-requests, rebase vs merge, cherry-pick, hooks, git flow)
- Code Intelligence (SonarQube, CheckStyle, FindBugs, pyLint)
- Code Coverage (JaCoCo, Cobertura)
- Cloud (cloud-native, infrastructure as a code)
- Docker & K8s (Dockerfile, docker build context, docker-compose, networks, sharing resources, k8s: pod, service, deployment)
- Performance (tools, concepts, isolation, bottlenecks, metrics, percentiles)
- Monitoring (Graphite, InfluxDB, Grafana)
- Reporting (Allure, ReportPortal)

## Practical

### Coding
- write recursive poller / classic poller
- write counter method for dict
- write simple decorator to track a time spent for method
- write method which check that int list contains only even values
- write method which check that string json has correct open-close brackets

### Selenium
- Get text of elements (ex. table) and create a dict with it (extra: build a model for this)
```html
<html>
  <body>
     <table>
        <tr>
           <th>First name</th>
           <th>Last name</th>
           <th>Age</th>
        </tr>
        <tr>
           <td>Jill</td>
           <td>Smith</td>
           <td>50</td>
        </tr>
        <tr>
           <td>Eve</td>
           <td>Jackson</td>
           <td>94</td>
        </tr>
     </table>
  </body>
</html>
```
- Fill all the inputs in the form
```html
<html>
  <body>
     <div class="form">
        <div class="input">
           <label>Input - 1</label><br>
           <input class="form_input" name="1" type="text">
        </div>
     </div>
     <div class="input">
        <label>Input - 2</label><br>
        <input class="form_input" name="2" type="text">
     </div>
     </div>
     <div class="input">
        <label>Input - n</label><br>
        <input class="form_input" name="n" type="text">
     </div>
     </div>
     </div>
  </body>
</html>
```
- Click behind the loader (what will be? how to avoid?)
- Login with API (how to implement?)
- Write/describe a simple page object
- Write/describe BasePage methods

### API
- Get ids of users who entered in September from the API response
```json
[
 {
   "id": "_4FG12Y7U6",
   "company": "Avionics Inc.",
   "firstname": "John",
   "lastname": "Doe",
   "entered": "2013-06-12T10:00:00Z"
 },
 {
   "id": "_4FG12Y7TX",
   "company": "Avis World Headquarters",
   "firstname": "Steve",
   "lastname": "Herbin",
   "entered": "2013-09-10T10:00:00Z"
 },
 {
   "id": "_4FG12Y7TV",
   "company": "BGP Productions",
   "firstname": "German",
   "lastname": "Vicencio",
   "entered": "2013-09-30T12:46:40Z"
 }
]
```
- Write/describe BaseApi methods

### SQL (dialect-dependent)
- Write UPDATE request
- Write INSERT request
- JOIN (types? differences? write request)
- Write request with COUNT
- Write request with GROUP BY
- Write request with HAVING
- Unique values (DISTINCT)
- Transactions

## Study plan
- Basic programming language course (OOP + Design patterns + Data structures + Code standards/conventions)
- Test framework (TestNG/JUnit - Java Pytest - Python)
- Selenium
- Page Object
- API automation
- DB automation
- Git
- Build systems (Maven/Gradle - Java pip/pipenv - Python)
- Jenkins
- Docker
- CodeCoverage/CodeIntelligence
