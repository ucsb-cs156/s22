---
num: "Lecture 18"
lecture_date: 2022-05-10
desc: "Tue Lecture: The Product Owner/Manager role"
ready: false
---

{% include drop_down_style.html %}


# Announcements

* H07 was due last night (Monday 05/09) at midnight, but there is a grace period until Midnight tonight (05/10).
* We'll likely start team03 (front end CRUD operations) tomorrow night in section.
* If you missed last Thursday's lecture, if you missed see last week's lecture on Thursday, the [video is here](https://gauchocast.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=6a3feb86-018d-4ff9-9212-ae8e015108de).


# Project Manager / Product Owner

In this lecture, Kevin Heffernan will talk a little about product manager/product owner roles on an Agile software development team.

We'll then do some product owner/manager type work on one of two applications:

| Section | Team 1 | Team 2 | Team 3 | Team 4 |
|--------------------|--------|--------|--------|--------|
| 4pm | s22-4pm-1: Courses | s22-4pm-2: Courses | s22-4pm-3: HappyCows | s22-4pm-4: HappyCows | 
| 5pm | s22-5pm-1: Courses | s22-5pm-2: Courses | s22-5pm-3: HappyCows | s22-5pm-4: HappyCows | 
| 6pm | s22-6pm-1: Courses | s22-6pm-2: Courses | s22-6pm-3: HappyCows | s22-6pm-4: HappyCows | 
{:.table .table-sm .table-striped .table-bordered}


In team01 and team02, you worked with a Kanban board populated with issues (cards).

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

There are two version of this exercise.  Please click the triangle to open up the one that pertains to your team.

| Section | Team 1 | Team 2 | Team 3 | Team 4 |
|--------------------|--------|--------|--------|--------|
| 4pm | s22-4pm-1: Courses | s22-4pm-2: Courses | s22-4pm-3: HappyCows | s22-4pm-4: HappyCows | 
| 5pm | s22-5pm-1: Courses | s22-5pm-2: Courses | s22-5pm-3: HappyCows | s22-5pm-4: HappyCows | 
| 6pm | s22-6pm-1: Courses | s22-6pm-2: Courses | s22-6pm-3: HappyCows | s22-6pm-4: HappyCows | 
{:.table .table-sm .table-striped .table-bordered}


<details>
<summary>
Courses  
</summary>
 
We'll be looking at a piece of software produced by past UCSB CMPSC 156 students (specifically, from F20, W21, S21).

This piece of software is intended as an "improved version" of 

* <https://my.sa.ucsb.edu/public/curriculum/coursesearch.aspx>
 

There are four versions that you can look at:
 
First, there is the one implemented by the F20/W21/S21 CS156 students:
* Available here <https://proj-ucsb-courses-search.herokuapp.com/>
* Code: <https://github.com/ucsb-cs156-s21/proj-ucsb-courses-search>
* This one has quite a few features beyond the UCSB production app
* But not all of them have been fully realized, and some may contain bugs or parts that are incomplete.

A few things that the S22 version of the app offers:
* Basic course search (but for a wider range of quarters; it goes all the way back to 2009)
* Advanced course searches.  Some examples:
  - When was a course offered over time, and who taught it?
  - For a given professor, what did they teach over time?
* Statistics of various kinds for various courses. 
 

There was an intention to start offering the ability to put together "sample schedules" of courses (this feature requires login),
though it was never fully implemented.   Think about: if it were, what would you want it to look like?

| What | Link |
|------|------|
| Running Appllication | <https://proj-ucsb-courses-search.herokuapp.com> |
| Source Code |  <https://github.com/ucsb-cs156-s21/proj-ucsb-courses-search> |
| Backend API (Swagger) | <https://proj-ucsb-courses-search.herokuapp.com/swagger-ui/index.html> |
| Storybook of React Components | <https://ucsb-cs156-s21.github.io/proj-ucsb-courses-search-docs/storybook> | 
{:.table .table-sm .table-striped .table-bordered}

Then there are three versions implemented by the W22 CS156 students. You'll be assigned one of these code
bases as your starting point.   These are very much preliminary works in progress:

| W22 Section | S22 Section | Heroku | GitHub |
| 5pm | 4pm | <https://courses-w22-5.herokuapp.com/> |  <https://github.com/ucsb-cs156-w22/team04-w22-5pm-courses>  |
| 6pm | 5pm | <https://courses-w22-6.herokuapp.com/> |  <https://github.com/ucsb-cs156-w22/team04-w22-6pm-courses>  |
| 7pm | 6pm | <https://courses-w22-7.herokuapp.com/> |  <https://github.com/ucsb-cs156-w22/team04-w22-7pm-courses>  |
{:.table .table-sm .table-striped .table-bordered}

You'll see that so far, these apps offer CRUD applications for schedules, but no ability to add or delete courses from those
schedules.
 
Also for basic search, the applications offer the ability to search, but only the basic search, and you can only see the course
heading, not information about particular sections.  It turns out that one of the most difficult and fundamental problems in implementing
a course search app is converting the structure of the JSON that is returned by the UCSB Courses Search API into a structure that
can be used to populate a table like the ones you see on 
the [Official UCSB Courses Search](https://my.sa.ucsb.edu/public/curriculum/coursesearch.aspx), or the
[S22 Courses Search](https://proj-ucsb-courses-search.herokuapp.com).
 
As you think about what feature you could work on, you may also consider the features available to you on GOLD, 
and whether some of those features could be and/or should be added to these apps.

 
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

Finally, also open up the app you are inheriting from the W22 section, here:
 
| W22 Section | S22 Section | Heroku | GitHub |
| 5pm | 4pm | <https://courses-w22-5.herokuapp.com/> |  <https://github.com/ucsb-cs156-w22/team04-w22-5pm-courses>  |
| 6pm | 5pm | <https://courses-w22-6.herokuapp.com/> |  <https://github.com/ucsb-cs156-w22/team04-w22-6pm-courses>  |
| 7pm | 6pm | <https://courses-w22-7.herokuapp.com/> |  <https://github.com/ucsb-cs156-w22/team04-w22-7pm-courses>  |
{:.table .table-sm .table-striped .table-bordered}

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
that you'd like to prioritize in the new version of the application, and mark those in your document.

Also, choose someone that can present for your team.  
 
# Step 6: As a class, each team shares 1 or 2 of the ideas your team came up with

We'll come around to allow each group to spend time sharing their idea(s). 

One student (maybe two) from each team will have half a minute to share their idea with the class.

So, keep it short! This is a low presure exercise meant to be fun and not test your public speaking skills. 

At most share 2 ideas that your team felt would be high priority with the class. 

</details>

<details>
<summary>
Happy Cows
</summary>
 
# Setting up access to the Heroku Dashboard

Your team has its own deployment of the original Happy Cows code (written in Express/Node), at one of these links:


* <https://happycows-og-4pm-3.herokuapp.com/>
* <https://happycows-og-4pm-4.herokuapp.com/>
* <https://happycows-og-5pm-3.herokuapp.com/>
* <https://happycows-og-5pm-4.herokuapp.com/>
* <https://happycows-og-6pm-3.herokuapp.com/>
* <https://happycows-og-6pm-4.herokuapp.com/>

You should also find a Heroku Dashboard link for these.  We've added ONE member of your team; that member of your team should 
add all of the rest.  (If they are absent today, ask Prof. Conrad or Kevin to add someone else, and then they can add the rest.)

Kevin and Prof. Conrad have added one member of each team to the Heroku app for your team at the dashboard links below:

* https://dashboard.heroku.com/apps/happycows-og-4pm-3.herokuapp.com/access>
* https://dashboard.heroku.com/apps/happycows-og-4pm-4.herokuapp.com/access>
* https://dashboard.heroku.com/apps/happycows-og-5pm-3.herokuapp.com/access>
* https://dashboard.heroku.com/apps/happycows-og-5pm-4.herokuapp.com/access>
* https://dashboard.heroku.com/apps/happycows-og-6pm-3.herokuapp.com/access>
* https://dashboard.heroku.com/apps/happycows-og-6pm-4.herokuapp.com/access>

We've let that person know on your slack channel. They should add all of the other members of the team.

# Giving each member of your team admin access to the app.

Before you can get admin access to the app, you need to have logged into the app at least once.

So, each team member should login at the regular app link below, and then make a post in the slack channel indicating they have done so.


* <https://happycows-og-4pm-3.herokuapp.com/>
* <https://happycows-og-4pm-4.herokuapp.com/>
* <https://happycows-og-5pm-3.herokuapp.com/>
* <https://happycows-og-5pm-4.herokuapp.com/>
* <https://happycows-og-6pm-3.herokuapp.com/>
* <https://happycows-og-6pm-4.herokuapp.com/>

When each team member has logged in, then you can do the next step.  For this, it is easiest to do this at the CSIL prompt, because the
`mysql` client is already installed there; you won't need it except for this one step, so it's not worth it to install on your local machine.

Just login into CSIL, and then paste in this command:

```
   mysql -u xxxx --password=yyyy -h us-cdbr-east-05.cleardb.net -D zzzzz
```

Of course, the values `xxxx`, `yyyy`, and `zzzz` are not the real values.  You'll get the real values by visiting the Heroku dashboard for your app,
and revealing the Config Vars, like this.  Click the "Reveal Config Vars" button, and you should see values for: `DB_NAME`, `DB_USERNAME` and `DB_PASSWORD`.   The xxxx is the username, the yyyy is the password and the zzzz is the database name.  Fill those in, and hit return.


<img width="1012" alt="image" src="https://user-images.githubusercontent.com/1119017/166589488-73f2575b-dd0e-48e1-85ec-35cf1ecf88e7.png">

That should bring up a prompt like this one:

<img width="652" alt="image" src="https://user-images.githubusercontent.com/1119017/166590401-caec4c4d-2df5-401e-ae97-1462fc6e3a96.png">

Where you can then use a command like this to  list all of the users:

```
select * from users;
```

You should get output like this:

```
+----+-----------+-----------+---------------------+-------+--------------------------------------+---------------------+---------------------+
| id | firstName | lastName  | email               | type  | token                                | createdAt           | updatedAt           |
+----+-----------+-----------+---------------------+-------+--------------------------------------+---------------------+---------------------+
|  4 | Kev       | Heffernan | kheffernan@ucsb.edu | admin | e775aeb0-cb34-11ec-8d12-d5718fa24def | 2022-05-03 23:01:02 | 2022-05-03 23:01:02 |
| 14 | Phill     | Conrad    | phtcon@ucsb.edu     | admin | ffbfcaa0-cb34-11ec-8d12-d5718fa24def | 2022-05-03 23:01:43 | 2022-05-03 23:01:43 |
+----+-----------+-----------+---------------------+-------+--------------------------------------+---------------------+---------------------+
2 rows in set (0.071 sec)
```

If you see that all of the users listed should be made admins, you can use this command to set them all at once:

```
update users set type='admin' where 1;
```

Or, you can set them one at a time like this:

```
update users set type='admin' where id='4';
```


Once you are finished, you can type `exit` to leave the mysql prompt.

At this point, every member of your team should have admin access.  You can test this by visiting the url `/admin` on your site, e.g.

* <https://happycows-og-4pm-3.herokuapp.com/admin>
* <https://happycows-og-4pm-4.herokuapp.com/admin>
* <https://happycows-og-5pm-3.herokuapp.com/admin>
* <https://happycows-og-5pm-4.herokuapp.com/admin>
* <https://happycows-og-6pm-3.herokuapp.com/admin>
* <https://happycows-og-6pm-4.herokuapp.com/admin>

From there, you can experiment with both the admin and user features of the app.

 
</details>


# What happens next?
 
In a future exercise, we'll talk about User Stories
* [User Stories](https://ucsb-cs156.github.io/topics/user_stories/) `As a __ I can __ so that __`
 
You may be asked to take the high level ideas you came up with in this exercise, and turn them first into **User Stories**, and then into 
**issues on a Kanban board** with [**Acceptance Criteria**](https://ucsb-cs156.github.io/topics/agile_acceptance_criteria/).
  


