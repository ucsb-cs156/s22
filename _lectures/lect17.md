---
num: "Lecture 17"
lecture_date: 2022-05-05
desc: "Thu Lecture: Front End Development"
ready: false
---

# Announcements

Reminder about H07: start learning JavaScript!

# Front End Development

Today, we'll go over some JavaScript and front end development concepts.

First, here's a cheat sheet of useful stuff:


* All front end code is in the directory `frontend`.  This is mostly JavaScript code.
* The structure of the code comes from [Create React App](https://create-react-app.dev/). 
  - Create React App is a system for creating a front end only React app.
  - We started with that, and then tweaked it for our purposes, and connected it to our Spring Boot backend.

# Front end testing:
* `npm test` by default, runs the tests for code that has changed since the last commit.
* `npm test` gives you the capability to press `a` to run all of the tests
* `npm run coverage` does test case coverage using jest.  This tends to run pretty quickly (< 60 seconds).
* `npx stryker run` does mutation testing for the frontend code using Stryker-js.  This tends to take a very long time (5-10 minutes)

# Running on Localhost:

On localhost, we run the backend in one terminal window, and the frontend in a separate terminal window.

## The first time

The backend is started in the usual way:
* `mvn spring-boot:run`

For the frontend, start a separate terminal window, and then do this:
* `cd frontend`
* `npm install` (this is only needed the first time,  if `package.json` has changed, or if `node_modules` has to be recreated)
* `npm start`

## The normal case

Usually, it's just: 
* `mvn spring-boot:run` in one window (from root of repo)
* `npm start` in another window (from `frontend` directory).

# Accessing swagger endpoint

On localhost, there is a link to access swagger, but on Heroku, there is usually not.

To access it you can add `/swagger-ui/index.html` to the end of the URL.  Note that the `/index.html` is *required* in this case.

For example: <https://cs156-s22-starter-team03.herokuapp.com/swagger-ui/index.html>

# Codecov

Be sure to visit the codecov page corresponding to your repo, i.e.

* e.g. <https://app.codecov.io/gh/ucsb-cs156-s22/STARTER-team03>
* in general: <https://app.codecov.io/gh/ucsb-cs156-s22/your-repo-name-goes-here>

And go to the Settings page and change the default branch from `master` to `main`.

<img width="778" alt="image" src="https://user-images.githubusercontent.com/1119017/167019081-3a353bbe-2527-4020-8895-b736be72bf0b.png">


Then, you can get the badge (see `Badge` in left navigation), copy the Markdown version of the badge, and put it at the top of your README.md.

<img width="1227" alt="image" src="https://user-images.githubusercontent.com/1119017/167019137-0c686e94-f6ea-483a-8ea7-2a5a9f896456.png">


# Sample Data from UCSB Developer API

The UCSB Developer API provides access to various kinds of data.  Many of the endpoints can provide sensitive data, so they are protected and require 
higher levesl of approval and authorization, but some of them provide data that is not all that sensitive (i.e. it is generally available to the public)
and so the levels of approval are reduced.  These are marked as "auto-approved" endpoints.

I've created a credential for use ONLY of the students in CS156 S22 and have provided it on the slack for the course.  This should only be used for
course activities (I will invalidate it with the course is over; if you want to continue using the APIs after that, please apply for you own credential.)

Here is the list of APIs you can access with this credential:

<img width="426" alt="image" src="https://user-images.githubusercontent.com/1119017/167021777-ff93e342-c945-4428-9424-2316e30e7326.png">


For this demo, we may need some sample data.  Here is some sample data for UCSB Dining Commons, from the UCSB Api.

* <https://developer.ucsb.edu/apis/dining/dining-commons#/info/GetInfoForAllDiningCommons>

We can access this at the command line using `curl` like this:

```
curl -X 'GET' \
  'https://api.ucsb.edu/dining/commons/v1/' \
  -H 'accept: application/json' \
  -H 'ucsb-api-key: put-the-consumer-key-here'
```  

The endpoint gives us this data (if supplied with a valid API consumer key):

```json
[
  {
    "name": "Carrillo",
    "code": "carrillo",
    "hasSackMeal": false,
    "hasTakeOutMeal": false,
    "hasDiningCam": true,
    "location": {
      "latitude": 34.409953,
      "longitude": -119.85277
    }
  },
  {
    "name": "De La Guerra",
    "code": "de-la-guerra",
    "hasSackMeal": false,
    "hasTakeOutMeal": false,
    "hasDiningCam": true,
    "location": {
      "latitude": 34.409811,
      "longitude": -119.845026
    }
  },
  {
    "name": "Ortega",
    "code": "ortega",
    "hasSackMeal": true,
    "hasTakeOutMeal": true,
    "hasDiningCam": true,
    "location": {
      "latitude": 34.410987,
      "longitude": -119.84709
    }
  },
  {
    "name": "Portola",
    "code": "portola",
    "hasSackMeal": true,
    "hasTakeOutMeal": true,
    "hasDiningCam": true,
    "location": {
      "latitude": 34.417723,
      "longitude": -119.867427
    }
  }
]
```


