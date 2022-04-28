---
num: "Lecture 17"
lecture_date: 2022-05-05
desc: "Thu Lecture: "
ready: false
---

# BELOW HERE TO BE COPIED PASTED INTO NEXT WEEK'S CLASSS

# Project Manager / Product Owner

In this lecture, Kevin Heffernan will talk a little about product manager/product owner roles on an Agile software development team.

We'll then do some product owner/manager type work: 

We'll look at a few apps that each provide some functionality related to UCSB Courses Search

* The one implemented by the University: <https://my.sa.ucsb.edu/public/curriculum/coursesearch.aspx> 
* The one implemented by the F20/W21/S21 CS156 students: <https://proj-ucsb-courses-search.herokuapp.com/>
* The three implemented by the W22 CS156 students (very much preliminary works in progress):
  * <https://courses-w22-5.herokuapp.com/>
  * <https://courses-w22-6.herokuapp.com/>
  * <https://courses-w22-7.herokuapp.com/>

In team02, you are working with a Kanban board populated with issues (cards).

This is very real world.

But: in the real world, where do the issues (cards) come from?

That's todays' topic.

# High level outline of today's class meeting

* In plenary session (2:00-2:30pm)
  * 5 minutes: Conrad: overview of today's lecture
  * 10 minutes: Kevin Heffernan: presentation on Product management
  * 5 minutes: Conrad: overview of product management activity
* In teams: ~2:30-3:05
  * 7 minutes: standup
  * 8 minutes: Independent work on ideating stories
  * 4 minutes: Working with a partner to identify most important ones (list of 3)
  * 8 minutes: Identifying two most important issues in team 
  * 12 minutes: Sharing with class ( 1 minute per team )
* In teams: ~3:05-3:15
  * Work on team02
  
# Product Owner / Product Manager

We'll start today with a presentation by TA Kevin Heffernan about the Product Manager/Product Owner role in a software development team.

The short version is that a product owner is the "voice of the customer" on the team. Why is this important to you? Because more and more software engineers required to work on product with more organizations becoming decentralized.

They:
* Talk to customers, prospective customers, and end users about their needs
  - These are not necessarily the same.
  - The customer is the one that writes the check, that makes the buy/no-buy decision.
  - The end user is the person that actually uses the software.
* Work with the software development team to turn customer needs into "user stories" 
* The user stories are then turned into issues (aka cards on a Kanban board.)

Kevin will tell you more: [Slides](https://docs.google.com/presentation/d/1Q93KdwjsbL-86Vj2bXWsT1OHDV5UM-d0/edit?usp=sharing&ouid=115856948234298493496&rtpof=true&sd=true)

# Let's do some product ownerish stuff

What we are doing: spending some time thinking about how to design a web application

Why we are doing this: 
* Learning/Educational reasons:
  * Product design is an important skill
  * Good sw dev organizations involve developers in product design
* Practical reasons
  * We are doing a fresh start implementation of proj-ucsb-courses-search
  * Reason: we've found a much cleaner/simpler architecture; easier to learn, easier to add new features
   

## First Exercise: Thinking like an end user

We'll be looking at a piece of software produced by past UCSB CMPSC 156 students (specifically, from F20, W21, S21).

This piece of software is intended as an "improved version" of 

* <https://my.sa.ucsb.edu/public/curriculum/coursesearch.aspx>
* Features available to you on GOLD

A few things that the app offers:
* Basic course search (but for a wider range of quarters; it goes all the way back to 2009)
* Advanced course searches.  Some examples:
  - When was a course offered over time, and who taught it?
  - For a given professor, what did they teach over time?

There was an intention to start offering the ability to put together "sample schedules" of courses (this feature requires login),
though it was never fully implemented.   Think about: if it were, what would you want it to look like?

| What | Link |
|------|------|
| Running Appllication | <https://proj-ucsb-courses-search.herokuapp.com> |
| Source Code |  <https://github.com/ucsb-cs156-s21/proj-ucsb-courses-search> |
| Backend API (Swagger) | <https://proj-ucsb-courses-search.herokuapp.com/swagger-ui/index.html> |
| Storybook of React Components | <https://ucsb-cs156-s21.github.io/proj-ucsb-courses-search-docs/storybook> | 
{:.table .table-sm .table-striped .table-bordered}


## Step 1: As a group, organize the document into sections by user

* Please open the Google Document Folder 4/22/22 that was shared in the announcement Slack channel. Navigate to your team's document.
* If you didn't already, add your name to the top.
* Now, add six headers for each of your names, so that you each have a section of the document to enter some notes, e.g. 

  > ## Alice
  > Alice's notes here
  > 
  > ## Bob
  > Bob's notes here
  >
  > ## Chris
  > Chris' notes here
  >
  > etc.

## Step 2: As an individual explore the application (4 minutes)

Then, as individuals, spend 5-10 minutes doing this:

Next: Open up the application.   
* Spend a few minutes exploring the <https://proj-ucsb-courses-search.herokuapp.com> application and it's features. 
* Compare/contrast with <https://my.sa.ucsb.edu/public/curriculum/coursesearch.aspx> and GOLD
* Think about what would be valuable to you as a student.


## Step 3: As an individual make some notes (4 minutes)

Then, make some notes about what you see that is good, and what could be improved. Aim for 3 items. 

As you make notes, consider including screenshots.

* What features do you find the most valuable?
* What changes would you make to the user interface?
* What features are missing that you think would be valuable?

If you'd like to see a certain feature, consider mocking up a design of what the forms would look like.

If you'd like to see changes to a User Interface, consider making a screen shot, and then marking it up with
the changes you'd like to see.

## Step 4: With a partner, share your ideas (4 minutes)

With a partner, discuss some of the ideas you each came up with independently. 

Take turns, half a minute each pitching each other your ideas.

Then, choose your favorite two to share with the team.

## Step 5: As a group, discuss your lists (8 minutes)

Add a section at the top of the document with a header called "Group Discussion"

> ## Group Discussion
> Enter notes here
>
> ## Alice
> Alice's notes here
> 
> ## Bob
> Bob's notes here
> etc.

Invite each pair of students on the team to share their two ideas for the application.

One member of the group should make some notes about what there is consensus about, and where
there is disagreement.  

Note all eight ideas. 

Finally, choose two of the most important features
that you'd like to prioritize in the new version of the application.

Choose someone to present a feature. If desired, one other student on the team can present another feature. 

Each student will have a half minute to present thier idea to the class.

# Step 6: As a class, each team shares 1 or 2 of the ideas your team came up with

We'll come around to allow each group to spend time sharing their idea(s). 

One student (maybe two) from each team will have half a minute to share their idea with the class.

So, keep it short! This is a low presure exercise meant to be fun and not test your public speaking skills. 

At most share 2 ideas that your team felt would be high priority with the class. 

# What happens next?
In a future exercise, we'll practice refining the high level notes into
* [User Stories](https://ucsb-cs156.github.io/topics/user_stories/) `As a __ I can __ so that __`
* Issues on a Kanban board with [Acceptance Criteria](https://ucsb-cs156.github.io/topics/agile_acceptance_criteria/)


