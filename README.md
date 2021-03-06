# Celerio Angular Quickstart

[![Build Status](https://travis-ci.org/jaxio/celerio-angular-quickstart.svg?branch=master)](https://travis-ci.org/jaxio/celerio-angular-quickstart)

This Angular quickstart uses Angular Cli to create the application skeleton and Celerio 
to **reverse your relational database schema** and **generate** the Angular + Spring Boot code 
to access your database content. The generated code covers much more areas than a simple Hello World app (search,
pagination, validation, auto-complete, etc.) 

To generate an application from a sample database, follow the instructions from the [quickstart][] folder.
The following [screencast](https://www.youtube.com/watch?v=MBrgeykyTGs) shows you what to expect.

Take a look at the generated code for yourself. Out of this 
[sample SQL schema](https://github.com/jaxio/celerio-angular-quickstart/blob/master/quickstart-conf/01-create.sql),
we generate this [code](https://github.com/jaxio/celerio-angular-quickstart/tree/master/quickstart-generated), 
thanks to these [templates](https://github.com/jaxio/celerio-angular-quickstart/tree/master/pack-angular/celerio/pack-angular).

By default we use a sample H2 database schema. Using your own database schema and database engine 
is just a matter of configuration. Check as an example our instructions to [use MySQL][] instead of H2.

## About the project

Our goal is to provide solid code generation templates for advanced Angular CRUD web applications.

Code generation templates are written in [Velocity][] and interpreted by [Celerio][], an Open Source `code generator`
tool for data-oriented applications.

Here is the folder organization:

* [pack-angular](https://github.com/jaxio/celerio-angular-quickstart/blob/master/pack-angular) folder contains the Celerio code generation templates that are interpreted/copied by [Celerio][]. 
* [quickstart-conf](https://github.com/jaxio/celerio-angular-quickstart/blob/master/quickstart-conf) folder contains the minimal configuration that Celerio needs to generate this quickstart.
* [quickstart](https://github.com/jaxio/celerio-angular-quickstart/blob/master/quickstart) folder is where you can generate the quickstart.
* [quickstart-generated](https://github.com/jaxio/celerio-angular-quickstart/blob/master/quickstart-generated): folder is an already generated quickstart provided here so you can browse the source code even from your phone :)

## About the generated code

The generated Angular CRUD web app uses the following technologies/frameworks:

* [Angular Cli](http://cli.angular.io/) a command line interface for Angular
* [Angular 4.0.0](http://angular.io/) web framework: we try to always use the most recent version
* [TypeScript](https://www.typescriptlang.org/): much easier than JavaScript... 
* [PrimeNG](http://primefaces.org/primeng/): Angular components library, we leverage file upload, auto-complete, calendar, tri-state checkbox, server-side pagination, etc.
* [Angular Material](https://material.angular.io/): Material Design components for Angular apps
* [Spring Boot](http://projects.spring.io/spring-boot/): Java app backend, made easy, we generate REST endpoints, etc.
* [Spring Security](http://projects.spring.io/spring-security/): basic security by default
* [Spring Data JPA](http://projects.spring.io/spring-data-jpa/): leverage query by example, etc.


## Contribute

You may contribute in several ways:

* By reviewing the generated code, are PrimeNG, Angular, Spring Data, Spring Boot, etc.  properly used ?
* By trying to generate a project using your own database schema
* By using the generated app and trying to find its limits

You may of course [report issues](https://github.com/jaxio/celerio-angular-quickstart/issues) and/or submit pull requests.


[generated quickstart]: https://github.com/jaxio/celerio-angular-quickstart/blob/master/quickstart-generated
[quickstart]: https://github.com/jaxio/celerio-angular-quickstart/blob/master/quickstart
[AOT instructions]: https://github.com/jaxio/celerio-angular-quickstart/blob/master/quickstart/README-AOT.md
[use MySQL]: https://github.com/jaxio/celerio-angular-quickstart/blob/master/quickstart/README-MYSQL.md
[Celerio]: https://github.com/jaxio/celerio
[Velocity]: http://velocity.apache.org/
