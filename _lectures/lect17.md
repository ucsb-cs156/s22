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
