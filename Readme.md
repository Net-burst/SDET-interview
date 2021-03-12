# AQA interview questions

## Purpose
The purpose of the interview is to determine level of hard and soft skills and to check 
that person fits team mentally.

## Approach
- prefer open questions: ie. questions without one correct answer
- when asking binary questions, mix yes and no questions. Don't coerce everything into yes or no

## Structure
- greeting and small-talk
- project introduction
- soft skills (past experience, English level, etc.)
- hard skills
- Q&A

## Soft skills
- Role on previous project
- Development methodology (Scrum, Kanban, Warefrall)
- QA process (code review, code intelligence, CI/CD)
- Good/bad practices
- Ideal QA/delivery process
- Notable tools

## Theory
Explain **what**, **when** and **why**.

### Computer science
- OOP (4 principles, basic use cases)
- Data Types (mutable/immutable) (primitives vs objects)
- Data Structures (collections, streams, iterators)
- Patterns / Anti-patterns
- SOLID, DRY, YAGNI
- Algorithms (Big O notation, basic algorithms)
- Test framework design/architecture (basic approaches, organization, must-use patterns)
- Limiting test run time and resource utilization / test run optimization

### Java
- primitives/objects
- mutable/immutable
- var (if Java 11)
- interfaces vs abstract classes
- annotations
- override/overload
- lambdas
- generics
- collections
- list/set/map
- hash map/hash set
- stream
- exceptions
- try/catch/finally
- static (method, variable)
- final (class, method, variable)
- access modifiers (default for class, interface)
- constructor/initializer
- equals and hashCode
- optional
- jUnit/TestNG/... (annotations, configuration, parallel run, parametrization)
- Maven/Gradle/... (role, configuration, dependencies, plugins, phases)

### Python
- mutable/immutable data types
- constructors (how to implement?)
- tuple vs list vs set
- list/dict comprehension
- the difference between v2 and v3
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
- keyword **pass**
- copy/deepcopy
- keyword **with** (context manager)
- keyword **yield**

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
- Element not clickable at point
- Download/upload file
- JS executor
- Actions
- Parametrized locator

### XPath
- Differences / and // 
- Differences . and ..
- Wildcard *
- Keyword contains
- Search by text
- Get parent element

### REST
- methods
- differences between PUT and POST
- PATCH, HEAD, OPTIONS
- components (verb, header, body, etc)
- supported markup languages
- status codes

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
- basic syntax
- joins
- subqueries
- grouping
- transactions
- CAP theorem
- ACID

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
