# Tech Stacks Read & Report
To help you get more experience with the idea of a tech stack and how different pieces of technology are selected and fit together to create a cohesive whole for a given project, we'll be doing a Read & Report exercise.

## Instructions
### Research
In this Read & Report exercise you will collaborate with your group to assign one or two particular technologies from the stack to each group member. Afterwards everyone will research their assigned technologies and try to learn the following:

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
Below we present four different tech stacks for previous Ada capstone projects. The technology choices listed here are based on the available code from those projects and may not reflect the complete set of technologies that were used. If your assigned tech stack has fewer technologies you should take the opportunity to investigate each technology in more detail.

Some of the technologies listed below fill the same role as the languages, libraries, and frameworks that we've learned already at Ada. When you find a technology that represents an alternative to, for example, Ruby you should make sure to compare and contrast it with the technology we've already used.

We've selected two mobile applications and two web applications:

### A. iOS native app
This tech stack includes the following components:
* Mobile App
  * Swift
  * Xcode
  * Google Maps API
  * Firebase

### B. iOS/Android cross-platform mobile app
This tech stack includes the following components:
* Mobile App
  * Flutter or React Native
  * Redux for in-app data management
  * Jest
* Back-end
  * Ruby on Rails
  * Web scraping
  * Nokogiri & HTTParty (for web scraping)

### C. Django web application
This tech stack includes the following components:
* Web front-end
  * jQuery
* API back-end
  * Python
  * Django
  * Indeed API
  * Postgres

### D. MEAN stack web application
This tech stack includes the following components:
* Web front-end
  * AngularJS
  * D3 visualization library
* API back-end
  * Node.js
  * Express
  * Seattle food inspection database
  * MongoDB
