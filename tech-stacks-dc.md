# Tech Stacks Divide & Conquer
To help you get more experience with the idea of a tech stack and how different pieces of technology are selected and fit together to create a cohesive whole for a given project, we'll be doing a Divide & Conquer exercise.

## Instructions
### Research
In this Divide & Conquer exercise you will collaborate with your group to assign one or two particular technologies from the stack to each group member. Afterwards everyone will research their assigned technologies and try to learn the following:

* What role does the technology play in a tech stack?
* What interface does the technology present to other technologies that will interact with it?
* What constraints does the technology place on the rest of the stack?

#### Example: **PostgreSQL**
* Its role is to provide relational data storage.
* It presents an interface that uses the SQL language for communicating queries to, and data from, the database.
* One of the constraints it places on the rest of the stack is that it must be hosted on a server that is accessible to all other parts of the tech stack that will use the database.

#### Example: **Stripe**
* Its role is to provide a service for managing everything related to real-money payments.
* It presents a RESTful, JSON Web API for communicating with its external service.
* Stripe has a number of different SDKs which are designed to work for web, mobile, and other use cases. By its design the only constraint that Stripe places on your tech stack is that whatever device the user makes payments with must have access to the internet.

### Presentation
Once everyone has researched their assigned technologies your group will come together again to discuss how each technology in the stack integrates with the other technologies and plan out how to present what is contained in the tech stack to the rest of the class.

You will need to create three presentation slides using Google Slides (details will be provided by your instructor). On your three slides you should present an overview of the tech stack as a whole and also dive into the major technologies being used.

## Example Tech Stacks
Below we present four different tech stacks for real-world applications. What we're presenting below is somewhere between the reality of the projects being hosted and an outside observer's hypothesis of what stack they are using. While each of these projects has a core piece that is open source most of them involve some proprietary software and/or hosting, which makes it difficult to say for certain what technologies are being used for that part of the stack.

### 1. [OneBusAway](http://onebusaway.org/) for iPhone
This tech stack includes the following components:
* [OneBusAway iPhone App](https://github.com/OneBusAway/onebusaway-iphone)
  * Swift
  * PromiseKit
  * Pulley
* [OneBusAway REST API](http://developer.onebusaway.org/modules/onebusaway-application-modules/current/api/where/index.html)
  * Java
  * Tomcat
  * Struts
  * Hibernate
  * HSQLDB
  * Apple Push Notifications
  * Spring
  * JUnit
  * Hessian

This document on [developing the OneBusAway server](https://github.com/OneBusAway/onebusaway-application-modules/wiki/Developer-Guide) may prove useful in understanding how the REST API's components fit together.

### 2. [F8 Conference App](https://github.com/fbsamples/f8app)
This tech stack includes the following components:
* Mobile App
  * React Native
  * Relay
  * Moment
  * Jest
  * Art
* Back-end
  * Node.js
  * Express
  * Parse Server
  * MongoDB
  * GraphQL

### 3. [Travis CI](https://travis-ci.org/)
This tech stack includes the following components:
* Web front-end
  * Ember
  * Broccoli
* API back-end
  * Ruby
  * Nginx
  * Sinatra
  * Memcached
  * PostgreSQL
  * Redis
  * Customer.io
  * RabbitMQ
  * RSpec
  * Factory Girl
  * Mocha (Ruby)

Travis CI is split up into several different pieces and [this document](https://github.com/travis-ci/travis-ci#README) has a great overview of them.

### 4. [SoundRedux](https://soundredux.io/)
This tech stack includes the following components:
* Web front-end
  * React
  * Redux
  * SoundCloud API
  * Local storage
  * Babel
  * Webpack
  * Mocha (JavaScript)
  * Nock
  * Lodash
  * ESLint
