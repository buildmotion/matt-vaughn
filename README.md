# Matt Vaughn

A repository for bio and other information about conference talks.

## BIO

Matt Vaughn built his first web application in 1998. Since then he's seen a few technologies come and go. However, his interest has always been to deliver high-quality solutions using SOLID principles and enterprise patterns. Matt leverages his architectural experience from full-stack development to create modern front end architecture using Angular and TypeScript. He is the author of the Angular Architecture book.

### Long Bio

Matt is a native of Colorado, USA. He has a passion for jazz, tacos, and of course technology. He has played the sax for many years and is starting to compose again in his home studio.

Matt Vaughn built his first web application in 1998. Since then he's seen a few technologies come and go. However, his interest has always been to deliver high-quality solutions using SOLID principles and enterprise patterns. Matt leverages his architectural experience from full-stack development to create modern front end architecture using Angular and TypeScript. He is the author of the [Angular Architecture](https://leanpub.com/angular-architecture-the-unofficial-guide) book.

Matt is also the host of the [Angularlicious Podcast](https://angularlicio.us/podcast) - a show about Angular, enterprise patterns and practices, and also Angular architecture. Matt speaks at local meetups and other conferences in Denver, Chicago, and Florida. Last year, he gave a workshop on the Angular Workspace at the [Angular Connect conference in London 2019](https://angularconnect.com/talks#matt-vaughn).

- **website**: [https://angularlicio.us](https://angularlicio.us)
- **blog**: [https://medium.com/@angularlicious](https://medium.com/@angularlicious)
- **podcast**: [https://angularlicio.us/podcast](https://angularlicio.us/podcast)
- **book**: [https://leanpub.com/angular-architecture-the-unofficial-guide](https://leanpub.com/angular-architecture-the-unofficial-guide)

## Workspace Superpowers

Learn what the new Angular Workspace offers developers and teams to create an efficient workflow. Learn best practices for working with many applications and libraries in a single environment. This presentation demonstrates how the Workspace supports good programming practices (DRY) and principles (Separation of Concerns). You will learn:

- the capabilities of the Angular Workspace
- if a monorepo is right for you?
- how shared configurations simplify maintenance
- to leverage the capabilities of the Nrwl.io Nx Workspace to publish libraries

The Angular Workspace is probably the biggest game changers in the workflow of Angular developers. This feature provides the backbone of sharing and reusing code as libraries. The new library project type provides capabilities to create:

- cross-cutting concern libraries
  - logging
  - error handling
  - configuration
  - notifications
  - security
- shared component libraries
- domain service libraries that supports domain-driven design
  - encapsulated business logic
- micro-applications/frontends to compose applications

### Notes for Workspace

> Note: I can also give a shorter presentation on this topic as well. I have given this presentation several times as a mini-workshop.

I began my journey into Angular by first determining if I could create reusable libraries to implement robust business logic. I created the Angular [Business Actions](https://github.com/angularlicious/angularlicious/tree/master/angularlicious-workspace/libs/actions) and [Rule Engine](https://github.com/angularlicious/angularlicious/tree/master/angularlicious-workspace/libs/rules-engine) frameworks using TypeScript. I was able to implement these NPM packages as TypeScript libraries. I focused on library projects as the mechanism to share and reuse code that would simplify the code base of one or more Angular applications.

The workflow for publishing npm packages or libraries is complex and developer resource intensive. I wrote a guide on how to do this back in 2018. The workflow and development environment was significantly enhanced with the release of Angular version 6 (May 2018). The new workspace or monorepo allows for multiple application projects and multiple library projects to be managed in a single environment. [Now my library arsenal includes](https://github.com/angularlicious/angularlicious/tree/master/angularlicious-workspace/libs):

- actions
- configuration
- contentful
- core
- error-handling
- firebase
- foundation
- http-service
- logging
- rules-engine
- security

The Angular Workspace has allowed me and the teams that I work on to focus on the solutions by sharing and reusing code with other library projects and all of our applications. The feature allows us to be more effective and efficient and to deliver high-quality apps that are extensible and maintainable. I have been able to take a team struggling with code consistency, consolidated logging, and error-handling issues to deliver stable and reliable production applications very quickly. Standing up new applications has also proven to be a benefit of the monorepo/Workspace. I compare it to development by the village. Each team member is a citizen, contributor, and maintainer of the village. We have a consolidation of efforts for the following:

- linting rules for formatting
- linting for consistency and syntax issues
- common pre-commit and pre-push hooks for Git
- a playbook of information for the developers that includes recipes, environments, workflows, etc.

It is allowing us to define best practices and have an environment (i.e., village) to use them. Much of this information is in my new book: [Angular Architecture available on LeanPub](https://leanpub.com/angular-architecture-the-unofficial-guide).

## Cross-Cutting Concerns

The default error handling and logging capabilities for an Angular application do not provide the critical information needed to monitor the health of an application once it is released to production. These (2) custom libraries have proven to be immensely valuable not only in production but also during development.

I feel that many cross-cutting concerns are not considered as part of the application's design or architecture. I have leveraged practices that were once only possible in the back end, now with Angular, TypeScript, and library projects we can create robust systems with the power of cross-cutting concerns.

### Long: Cross-Cutting...

Where should I put my plumbing or infrastructure code in my application? Application domain features use these aspects - but they are not related to the specified feature. What are the best practices for implementing cross-cutting concerns? Where should they be located and how can I share them between multiple applications and projects? Learn to manage and separate cross-cutting concerns from your applications to improve modularity.

Learn what a cross-cutting concern is and how to identify one. The presentation demonstrates practices to implement, load, configure and use cross-cutting concerns. Take advantage of the monorepo approach (Angular Workspace) and custom libraries.

- Learn strategies, concepts, and patterns to create and reuse these cross-cutting concerns in multiple applications.
- Cross-cutting Concerns:
  - Configuration
  - Exception Handling
  - Logging services, writers, and formatters; logging providers
  - Security authentication/authorization
  - Notifications
  - HTTP/Data Access
  - Data Validation and Business Rule processing
- Learn best practices and guidelines for implementing

### Notes for Cross-Cutting Concerns

I have been developing web-based applications since 1998. Many of these years, I focused on architecture, enterprise patterns, and practices; as well as Object-Oriented programming. As a consultant, I have worked with many different domains from travel, hospitality, medical, and financial. I have learned that there are many elements of an application that are the same without regard to the specific domain or industry.

My question is why do many development teams not consider cross-cutting concerns as first-class elements in their design and plans. They provide essential features for applications. Many times, these cross-cutting concerns are implemented inline with the production/feature code. When this happens, there is little potential for reuse or maintenance.

This presentation or workshop provides the information for Angular and/or web application developers to begin discussions, planning, and implementation of crosscutting concerns. Each attendee should walk away understanding the importance of at least (3) of many cross-cutting concerns:

1. logging
2. error handling
3. configuration

## Architecture to the Cleaners

In software, some times you only have one chance to get it right. It is possible with a well-defined architecture. Maximize the capabilities of Angular, Typescript, Visual Studio Code tools to enable architectural patterns that were once not available or easy to implement in modern web applications.

During this session, we will cover how to apply CLEAN and SOLID principles to Angular applications to simplify your application code base and maximize your code sharing and reuse. A reference application will also demonstrate a reactive design approach using the powers of RxJS.

### Long: Architecture...

This talk presents a layered or n-tier approach for Angular applications. Many Angular applications do not apply the Single-Responsibility or Separation of Concerns principles as much as they can. Therefore, the components and services are doing way too much. This talk demonstrates how to use very common architectural patterns along with the Angular Workspace to create layers with distinct responsibilities. Many of these strategies fall under the category of good code organization.

The result is a simplified code base that allows for greater extensibility and easier maintenance of the application.

### Notes for Arch

I spent about 16 years of my career focused on full-stack web application architecture. Many of the patterns and practices were implemented on the backend using Object-oriented languages like C#.

There were always good coding practices for HTML, CSS and JavaScript. However, JavaScript is not an OOP language. With Angular and TypeScript we have new capabilities. TypeScript provides us with all of the OOP features we need to implement designs and architectures that were not possible before TypeScript (maybe possible, but way more difficult).

Since 2016, I have been learning how to apply layered/n-tier designs for web applications (Angular). I have compiled all of this information in a new book: [Angular Architecture available on LeanPub.com](https://leanpub.com/angular-architecture-the-unofficial-guide).

My goal is to not sell books, but to share information on how we can improve web application architecture with the modern tool-sets that we have. I provide my book for free at conferences and meetups, I have also donated over 40 books to NgGirls last year.

The tools we have today didn't exist a few years ago. I am amazed at the Angular community and the pace that it keeps delivering tools to make it even better.
