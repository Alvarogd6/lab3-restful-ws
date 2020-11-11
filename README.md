[![Build Status](https://travis-ci.com/UNIZAR-30246-WebEngineering/lab3-restful-ws.svg?branch=master)](https://travis-ci.com/UNIZAR-30246-WebEngineering/lab3-restful-ws)
# Web Engineering 2020-2021 / RESTful Web services
**In this assignment your PR must only modify the `README.md` file**.
Please, go to the [Wiki](https://github.com/UNIZAR-30246-WebEngineering/lab3-restful-ws/wiki) in order to get the instructions for this assignment.

## Primary goal

Complete the tests of `AddressBookServiceTest` to tests if the service meets the HTTP semantics.
Each test in `AddressBookServiceTest` is incomplete. 
For example, the method `serviceIsAlive` tests if: 

```http
GET /contacts
```

returns an empty list, but it must be extended in order to verify that `GET /contacts` meets the HTTP GET contract: 

- GET request is safe (it does not modify the contents of the address book)
- GET request is idempotent (two consecutive calls return the same).

## Secondary goals (:gift:)

Solutions must meet primary goals too. 

Proposed:

- Replace the current implementation (Jakarta Jersey) by a [Spring MVC](https://docs.spring.io/spring-framework/docs/current/reference/html/web.html#spring-web) (Servlet) implementation
- Replace the current implementation (Jakarta Jersey) by a [Spring WebFlux](https://docs.spring.io/spring-framework/docs/current/reference/html/web-reactive.html#spring-webflux) (Reactive) implementation
- Support asynchronous requests without using Spring WebFlux 
- Use [JWT credentials](https://jwt.io/) to grant access to requests
- Support of [CORS](https://developer.mozilla.org/es/docs/Web/HTTP/Access_control_CORS) requests 
- Support of HTTP/2 requests 
- Support of HTTPS requests using self-signed certificate 
- Support of OpenAPI 3.0

Note: unless the goal specifies o disallows a specific framework you are free to replace the framework used in the original implementation with a different framework.

Manifest your intention first by a PR updating this `README.md` with your goal.
If you desist of your goal, release it by a PR so other fellow can try it. 


| NIA    | User name | Repo | Build Status | Improvement | Score
|--------|-----------|------|--------------|-------------|--------
|        |           |      |              |             |
| 760704 |[Álvaro García](https://github.com/Alvarogd6)|[Alvarogd6/lab3-restful-ws](https://github.com/Alvarogd6/lab3-restful-ws/tree/test)|![Build Status](https://travis-ci.com/Alvarogd6/lab3-restful-ws.svg?branch=test)|             |