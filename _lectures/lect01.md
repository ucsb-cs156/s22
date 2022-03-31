---
num: "Lecture 01"
lecture_date: 2022-03-30
desc: "Wed Section"
ready: true
---

Today's section is an opportunity to get started on two programming assignments.

During section, you may turn to any of the staff for help.  But we have the following mapping from staff to teams as the "default" mapping, i.e. the staff member that you turn to first:

* 4pm-1, 5pm-1. 6pm-1: Andrew Lu
* 4pm-2, 5pm-2, 6pm-2: Andrew Peng
* 4pm-3, 5pm-3, 6pm-3: Bryan Zamora Flores
* 4pm-4, 5pm-4, 6pm-4: Kevin Heffernan


The first is quite straightforward; just a "Hello World" program in Java.

The second is a bit more involved; it includes an introduction to:
* Unit testing in Java with JUnit
* Code Coverage using Jacoco
* Mutation Testing using Pitest

# Why a Hello World Program?
* To ensure that you have access to a Java compiler
* To ensure that your GitHub and Gradescope accounts work
* To take care of mechanical issues before we start tackling real programming

# Why an assignment on testing?

* Testing is a fundamental component of professional software development
* In particular, we want to learn something called CI/CD: Continuous Integration, Continuous Delivery
* You can think of CI/CD as similar to a "professional level autograder"
  - As with autograded assignments, there is a set of tests that are run against the code
  - If the tests pass, the code is assumed to be in a good state to deliver to customers
  - Professional organizations use CI/CD as a way to speed up delivery, and ensure quality
* But unlike autograders, which seems to come from "on high", professional developers have to maintain their own tests
  - In an academic course, the test cases usually come from the instructor
  - In a real world setting, the team that develops the software also *develops the tests*
  - How do we know if our tests are any good?
  - There are tools for this: code coverage and mutation testing.

# I'm just a beginner in Java !?! Where can I get help?

There are three mainresources for you to learn Java:

* The `Student` tutorial set up by the instructor, available here: <https://ucsb-cs156.github.io/tutorials/student/>
  - This tutorial takes you through a variety of topics in Java, using a simple `Student` class as the basis.
* The Head First Java textbook, while really old and very out of date with many later Java features, is still a great way to learn many of the fundamental concepts of Java:
  - How objects work in Java, including some of the major differences between Java and C++
  - Inheritance vs. interfaces (`extends` vs `implements`)
  - Exception handling
  - Wrapper types (`Integer` vs. `int`, `Boolean` vs. `boolean`, etc)
  - and much more
* The Java in a Nutshell version 7 book.  This book has more about the later features of java, including:
  - Annotations (the things that start with `@`)
  - Lambda Expressions (the things that have an arrow `->` in them)

In addition, you can get help from the Course Staff, via the Slack
* For each assignment, there will typically be a `#help` channel, e.g. `#help-jpa00`, `#help-jpa01`, etc.
* You can ask for help there.
* During lecture or section, use the `#help-lecture-discussion` channel instead; the staff treats this as a kind of "help queue" to make sure that we get to as many students as possible.

 
