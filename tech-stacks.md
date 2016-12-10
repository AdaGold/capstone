# Capstone Technology Features
One of the most exciting and challenging things about the capstone project is learning new technologies to integrate into your project.

## Technology Stacks
Real-world projects are composed from a selection of specific technologies that each take care of some piece of the work necessary to have a production-ready application. The full set of technologies that are used in a project is known as the **technology stack** for that project. For your capstone project you'll need to determine what tech stack you should use, based on the needs of your project plan.

### Major Parts of a Web Application Tech Stack
Every project's goals are different, and as a result its tech stack will be different. However, within the realm of web applications there are several major pieces that virtually every project requires:

* Back-end
  * Web application framework
  * Web server
  * Database server
  * Authentication framework
* Front-end
  * JavaScript framework
  * CSS library (or language)
  * Internationalization (i18n)
  * Mobile framework/language
* Web infrastructure
  * Server hosting
  * Content delivery network
  * DNS hosting/management
  * SSL certificates
* Code infrastructure
  * Continuous Integration
  * Code quality/linting tools
* DevOps systems
  * Provisioning
  * Orchestration
  * Monitoring

We've already seen many technologies that fill several of these roles. For example, Rails is a **Web application framework**. It has a built-in **Web server** which we've used, however there are a number of alternatives including [Puma](http://puma.io/) which is now the default in Rails 5. What roles are filled by some of the other technologies we've used?

A couple of the technologies listed above are possibly new to you because we've not had to implement them for our projects so far. For example, both DNS hosting and SSL certificates were handled for us by Heroku when we deployed our Rails applications. In more complex deployment scenarios these, and many other, tasks must be handled by either the developers or a DevOps team working closely with them.

### Project-specific Technologies
In addition to the technologies listed above other technologies are often added to a stack because of specific needs from the project.

For example, if the application allows users to pay for items or services (such as an e-commerce site) the technology stack would need to include a payment processing service such as [Stripe](https://stripe.com/). Here are some other technologies that are likely to be found in a web application tech stack:

* Service Oriented Architecture
  * API/Web service protocol ([REST](https://en.wikipedia.org/wiki/Representational_state_transfer), [SOAP / WSDL](https://en.wikipedia.org/wiki/Web_Services_Description_Language), [Apache Thrift](https://thrift.apache.org/))
  * Message/Job Queue ([Amazon SQS](https://aws.amazon.com/sqs/), [Apache ActiveMQ](http://activemq.apache.org/), [Apache Kafka](https://kafka.apache.org/))
  * [Service broker / repository](https://en.wikipedia.org/wiki/Web_Services_Discovery)
* External APIs
  * Data stores ([Socrata Open Data](https://dev.socrata.com/), [data.gov](https://www.data.gov/), [Seattle Open Data](https://data.seattle.gov/))
  * Services ([Google APIs](https://developers.google.com/), [Twilio](https://www.twilio.com/), [Stripe](https://stripe.com/))
* Real-time systems
  * [Voice Over IP](https://en.wikipedia.org/wiki/Voice_over_IP)
  * [Push Notifications](https://www.urbanairship.com/push-notifications-explained) ([iOS](https://developer.apple.com/notifications/), [Android](https://developer.android.com/guide/topics/ui/notifiers/notifications.html), [Web](https://developer.mozilla.org/en-US/docs/Web/API/Notifications_API))
  * [WebSocket](https://en.wikipedia.org/wiki/WebSocket)
* Data visualization & graphics
  * Charts ([High Charts](http://www.highcharts.com/))
  * General purpose ([D3](https://d3js.org/), [Processing.js](http://processingjs.org/))
  * [WebGL](https://en.wikipedia.org/wiki/WebGL) (Demo: [Chrome Experiments](https://www.chromeexperiments.com/webgl))
* Data management
  * Data storage ([Amazon S3](https://aws.amazon.com/s3/), [Google Cloud Storage](https://cloud.google.com/storage/))
  * [Content Management System](https://en.wikipedia.org/wiki/Content_management_system)

### Example Tech Stack
To get a better sense of everything comprised in a tech stack, here's an example of one using familiar technologies:

The PotBS Account Management Site Tech Stack:
* Back-end
  * [Ruby on Rails](http://rubyonrails.org/)
  * [Unicorn](https://bogomips.org/unicorn/) web server
  * [PostgreSQL](https://www.postgresql.org/) relational database
  * [Devise](https://github.com/plataformatec/devise) for user management & authentication
  * [Haml](http://haml.info/) for views (instead of ERB)
  * RESTful API
  * XML API
* Front-end
  * [jQuery](https://jquery.com/)
  * [Foundation](https://foundation.zurb.com/) CSS framework
* Web infrastructure
  * [Heroku](https://www.heroku.com/) hosting (back-end)
  * [Firebase](https://firebase.google.com/) hosting (front-end)
  * [MaxCDN](https://www.maxcdn.com/) for CDN hosting
  * [DNSimple](https://dnsimple.com/) for DNS management
  * SSL certificates purchased from [StartSSL](https://www.startssl.com/)
* External APIs
  * Proprietary account service API for PotBS game
  * [PayPal IPN](https://developer.paypal.com/docs/classic/products/instant-payment-notification/) API
  * [Mandrill](http://www.mandrill.com/) transaction email service
* Code infrastructure
  * [CircleCI](https://circleci.com/) for continuous integration
* DevOps systems
  * [New Relic](https://newrelic.com/) for real-time error monitoring
  * [Papertrail](https://papertrailapp.com/) for production log collection
