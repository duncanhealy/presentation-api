# Api  

## What

Application Programming Interface (API) In basic terms, APIs just allow applications to communicate with one another. ... An API is not a database. It is an access point to an app that can access a database.


## How 

An API is a software intermediary that allows two applications to talk to each other. In other words, an API is the messenger that delivers your request to the provider that you're requesting it from and then delivers the response back to you.


## Why do we use APIS

The development of apps for mobile devices meant that organisations needed to allow users to access information through apps and not just through the Internet. APIs are used to allow organisations to easily share information to many different systems.


## Where

10000?0s of APIS published for open consumption. This along with Open Data movements have shifted how we can consume and process data.


## When

APIs allow the movement of data in a structured manner from server to client and vice-versa



## Examples - Public APIS

- https://github.com/OAI/OpenAPI-Specification

- https://github.com/TonnyL/Awesome_APIs

- https://github.com/lorien/awesome-web-scraping

- https://github.com/marmelab/awesome-rest


- How many were you using without realising


## Documentation

  + Reading 
  + Experimenting to find out what they had not documented
  + Testing continuously for regressions
  + How can we make this a better experiece



## Protocols

- Text

- Custom formats

- Binary

- XML

- SOAP

- RPC

- JSON


- XML-RPC

- JSON-RPC

- GRPC

- socket 

- GraphQL

- DB



## API Types

- REST
- REACTIVE
- PUSH
- PULL
- CRUD
- Framework


## Protection + Security

- Authentication
- Oauth
- SAML
- JWT
- !COOKIES
- !Session
- Monitoring
- Realtime alerts
- Analysis


## Build in

- Rate limits
- Error handling
- http retry
- traffic shifting
- canary a/b



## Paradigms

- Frontend

- Middleware

- Backend

- SPA

- Serverless



## Microservices

- Monolith

- Microlith

- Microservices

- Nanoservices FAAS



# Deployment Targets

- Container

- Groups of Containers

- Groups of Groups



## Standardisation

- Serialisation
- Deserialisation
- Pass objects around 
- Documentation
  + https://github.com/unicodeveloper/awesome-documentation-tools


## Test Requests

  + https://httpbin.org


## Mock servers

  + https://mockoon.com/

  + https://www.mockable.io/

  + https://www.mocky.io/

  + https://learning.getpostman.com/docs/postman/mock_servers/setting_up_mock/


  + https://wiremock.org/

  + [json-server](https://github.com/typicode/json-server)

  + https://github.com/Marak/faker.js

  + https://github.com/json-schema-faker/json-schema-faker
  + https://rawgit.com/Marak/faker.js/master/examples/browser/index.html


## Testing

  + Selelium
  + mocha
  + load testing



## Tools



## Apigeneration

[Swagger UI](https://swagger.io/tools/swagger-ui/)

[Postman](https://www.getpostman.com/)

[openapi.tools](https://openapi.tools/)


## Postman

- Tests can be built in
- Documentation built in

```js
var jsonData = JSON.parse(responseBody);
postman.setEnvironmentVariable("access_token", jsonData.access_token);
pm.test('all ', () => {
    pm.test('json ', () => {pm.response.to.be.json;})
    pm.test('headers ', () => {pm.response.to.have.header('Content-Type', 'application/json; charset=utf-8');})
    pm.test('200 ', () => {pm.response.to.have.status(200);})
})
```


## Containers

- Docker - https://www.docker.com/

- Kubernetes - https://kubernetes.io/

- Netlify - https://www.netlify.com/


## Lint

Eslint - https://eslint.org/

JSHint - https://jshint.com/

JSLint - https://www.jslint.com/


## Code Testing Frameworks 

- Jest - https://jestjs.io/

- Jasmine - https://jasmine.github.io/

- Mocha - https://mochajs.org/

- Karma - https://karma-runner.github.io


## Code analyis

- https://en.wikipedia.org/wiki/List_of_tools_for_static_code_analysis
- https://www.owasp.org/index.php/Source_Code_Analysis_Tools


## Pipelines

- gitops flow 
- flux
- jenkins-x
- devops


## E2E

- Protractor - https://www.protractortest.org/

- Selenium - https://www.seleniumhq.org

- Cypress - https://www.cypress.io/

- TestCafe - https://devexpress.github.io/testcafe/


## CICD

- Jenkins - https://jenkins.io/

- Travis CI - https://travis-ci.org/

- CircleCI - https://circleci.com/


## Diagnostics 

- custom vs framework
- https://heptio.github.io/sonobuoy/latest/



## Standard Response 
  
  + https://tools.ietf.org/html/rfc7231#section-6

  + https://www.iana.org/assignments/http-status-codes/http-status-codes.txt


```txt 
    Value            Description                             Reference
     100   Continue                        [RFC7231]
     101   Switching Protocols             [RFC7231]
     102   Processing                      [RFC2518]
     103   Early Hints                     [RFC8297]
   104-199 Unassigned
```


```txt
     200   OK                              [RFC7231]
     201   Created                         [RFC7231]
     202   Accepted                        [RFC7231]
     203   Non-Authoritative Information   [RFC7231]
     204   No Content                      [RFC7231]
     205   Reset Content                   [RFC7231]
     206   Partial Content                 [RFC7233]
     207   Multi-Status                    [RFC4918]
     208   Already Reported                [RFC5842]
   209-225 Unassigned
     226   IM Used                         [RFC3229]
   227-299 Unassigned
```


```txt
     300   Multiple Choices                [RFC7231]
     301   Moved Permanently               [RFC7231]
     302   Found                           [RFC7231]
     303   See Other                       [RFC7231]
     304   Not Modified                    [RFC7232]
     305   Use Proxy                       [RFC7231]
     306   (Unused)                        [RFC7231]
     307   Temporary Redirect              [RFC7231]
     308   Permanent Redirect              [RFC7538]
   309-399 Unassigned
```


```txt
     400   Bad Request                     [RFC7231]
     401   Unauthorized                    [RFC7235]
     402   Payment Required                [RFC7231]
     403   Forbidden                       [RFC7231]
     404   Not Found                       [RFC7231]
     405   Method Not Allowed              [RFC7231]
     406   Not Acceptable                  [RFC7231]
     407   Proxy Authentication Required   [RFC7235]
     408   Request Timeout                 [RFC7231]
     409   Conflict                        [RFC7231]
```


```txt
     410   Gone                            [RFC7231]
     411   Length Required                 [RFC7231]
     412   Precondition Failed             [RFC7232]
     413   Payload Too Large               [RFC7231]
     414   URI Too Long                    [RFC7231]
     415   Unsupported Media Type          [RFC7231]
     416   Range Not Satisfiable           [RFC7233]
     417   Expectation Failed              [RFC7231]
     418   ?
   419-420 Unassigned
```


```txt
     421   Misdirected Request             [RFC7540]
     422   Unprocessable Entity            [RFC4918]
     423   Locked                          [RFC4918]
     424   Failed Dependency               [RFC4918]
     425   Too Early                       [RFC8470]
     426   Upgrade Required                [RFC7231]
     427   Unassigned
     428   Precondition Required           [RFC6585]
     429   Too Many Requests               [RFC6585]
     430   Unassigned
     431   Request Header Fields Too Large [RFC6585]
   432-450 Unassigned
     451   Unavailable For Legal Reasons   [RFC7725]
   452-499 Unassigned
```


```txt
     500   Internal Server Error           [RFC7231]
     501   Not Implemented                 [RFC7231]
     502   Bad Gateway                     [RFC7231]
     503   Service Unavailable             [RFC7231]
     504   Gateway Timeout                 [RFC7231]
     505   HTTP Version Not Supported      [RFC7231]
     506   Variant Also Negotiates         [RFC2295]
     507   Insufficient Storage            [RFC4918]
     508   Loop Detected                   [RFC5842]
     509   Unassigned
     510   Not Extended                    [RFC2774]
     511   Network Authentication Required [RFC6585]
   512-599 Unassigned
```



## Ready to Build

- Favourite Toolsets

- Frameworks



# Starting points

- https://katacoda.com/


- Good resources for futher reading

- https://blogs.mulesoft.com/dev/api-dev/what-is-api-led-connectivity/

- https://medium.com/aubergine-solutions/api-testing-using-postman-323670c89f6d

- https://jamesmessinger.com/postman-bdd/

- https://learning.getpostman.com/docs/postman/scripts/test_examples/


- http://jasonwatmore.com/post/2018/08/06/nodejs-jwt-authentication-tutorial-with-example-api

- https://k3s.io

- https://microk8s.io/

- https://cd.foundation/projects/

- https://docs.cert-manager.io/



## Security

- HSTS
- CORS
- https://github.com/OWASP/CheatSheetSeries/blob/master/cheatsheets/REST_Security_Cheat_Sheet.md
- https://docs.mongodb.com/manual/administration/security-checklist/
- https://www.mongodb.com/blog/post/how-to-avoid-a-malicious-attack-that-ransoms-your-data#suggested-steps



## Questions


- High level API design - how do we create collections, how do we
break it all down


- Use of functions, does the code tied to the route just do some
simple parsing and then call a function in terms of implementation, or
do you put as much logic as possible in the actual code?


- Pros and Cons of handling backend state vs passing it around as a parameter


- Testing suites for Postman for example - things to look for