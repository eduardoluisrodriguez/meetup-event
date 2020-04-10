# Meetup Event Planner

## About the App
The app consists of a Rails / GraphQL API and React Front End.  

A web application to arrange meetup events using cutting edge technologies, including GraphQL, Ruby on Rails and React.

Technical Milestones
- Integrated GraphQL on top of Ruby on Rails for the site's data layer
- Built an authentication system for the site
- Utilized UX best practices and built dynamic web forms to add to the interactivity of the site
- As always, followed the AirBnB JSX and JavaScript style guides and utilized ESLint to provide exceptional style and code quality.

## Getting Started
The repo contains two projects, seperated by subtrees.  The server bootstraps at the root level, whereas the Front End begins in the `./client` directory.

# Client

## Installing
The package.json file includes over a dozen npm scripts to make most tasks a breeze.

Installation can be achieved by running
```
npm run setup
```

To get the development server running, please run
```
npm run start
```

### Scripts

If you just want to serve the minified and chunked bundles, which might be faster, you can run
```
npm run serve:bundle
```

In production, the client connects to the heroku server.  You can run the server locally with the following command.
```
NODE_ENV=development node server
```

### Build
The application is bundled using Webpack and the production configuration includes many optimizations, including
- Code Chunking
- CSS Module Extract Text
- Minification / Uglification

### Testing
The test suite contains over 70 tests and can be run with
```
npm run test
```

### Deployment
The app is deployed to Heroku and has a CI suite running with Codeship.  It is running Express JS and GraphQL on the server for Front end and GraphQL on Rails for the back end

## API
### Getting started
The client app will by default connect to the live API.  If needed, you can get this API running following the guide below.

### Installation
Running the following commands in succession will effectively setup the API and get it up and running.
```
rvm use ruby-2.3.1@rails5.0 --create
bundle install
rake db:setup
rails s
```

## Troubleshooting
When working with a team on a project that uses Node, it is important that everyone use the same version of node and npm.
In the case of this project, we are using Node version 5.2.0.


## Screen Shots
![Meetups](https://github.com/RyanCCollins/cdn/blob/master/portfolio-image-gallery-images/meetup-event-planner/meetup-event-planner/main-mock.png?raw=true)
