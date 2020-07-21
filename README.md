# x-pent-up

The umbrella project to a simple personal financial budget application to learn Ember.js and Ruby on Rails development 
model along other interesting stuff. 

Check:
- [X Pent Up UI](https://github.com/alejoceballos/x-pent-up-ui) for the frontend project made in Ember.js
- X Pent Up API (TBD) for the back-end project made in Ruby on Rails

## Technology Stack Goals

### Process

- Single branch
- Feature flags

### Tech Stack
- PostgreSQL (db)

#### Ruby (language)
- Ruby on Rails (MVC framework)	
    - TwP/logging-rails
    - cerebris/jsonapi-resources	
    - mperham/sidekiq (asynchronous work)
    - krisleech/wisper (publish-subscribe capabilities)

#### Javascript (language)
- Typescript
- Ember.js (SPA framework)
    - DockYard/ember-composable-helpers
    - kategengler/ember-feature-flags
    - machty/ember-concurrency
    - machty/ember-concurrency-decorators
    - **miragejs/ember-cli-mirage:** Ember Mirage library that lets mock out backend APIs
    - offirgolan/ember-cp-validations
    - **simplabs/ember-test-selectors:** Auto `data-test-...` features for the project
    - yapplabs/ember-wormhole

#### CSS (language)
- Sass (framework)

#### Communication
- HTTP REST (Communication protocol)
    - JSON API (Data format specification)

- Amqp (Queue Protocol)
    - RabbitMQ (Queue manager)
  
#### Containerization  
- Docker

#### Version Control System
- Git
    - GitHub (Version control hosting platform)
	

#### Continuous Integration / Deployment
```
                           Frontend             Backend
+-------------------+--------------------+------------------+
| Linter            | Eslint             | Rubocop          |
| Unit Tests        | Ember/QUnit        | Rspec            |
| Integration Tests | Ember/QUnit        | Rspec            |
| Acceptance Tests  | Ember/QUnit/Mirage | Rspec            |
| Code coverage     |                    | SimpleCov        |
| Code quality      | SonarQube          |                  |
| Build             |
| Deploy            |
+-------------------+--------------------+------------------+
```
