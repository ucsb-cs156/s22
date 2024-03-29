---
num: "Lecture 18"
lecture_date: 2022-05-10
desc: "Tue Lecture: The Product Owner/Manager role"
ready: true
4pm_1_doc: https://docs.google.com/document/d/1GV_kSDt7VERaWURg2CcCNN4gYaSvABfMc1Li7LqAdEo/edit?usp=sharing
4pm_2_doc: https://docs.google.com/document/d/1AVEHExtlvL50uoiape9K97GKpYEijsGuVE7WncWKKbM/edit
4pm_3_doc: https://docs.google.com/document/d/1HAkiuL6HnTevcTu91Ncm8ir1xpxDIoO-L8w01WR_59c/edit
4pm_4_doc: https://docs.google.com/document/d/1EbWBf4NBVDdED0gPJp41TPNmEcvabt5V5CpX_NKwrIc/edit?usp=sharing
5pm_1_doc: https://docs.google.com/document/d/1RX5HzEyGF7Bgl5Ph701_D3jqOre3pkyR28UmcbiTq64/edit
5pm_2_doc: https://docs.google.com/document/d/1NQf6q9pCDWlIBNYQkGw9dy3caodlH2JLBa2NpNyEVXc/edit
5pm_3_doc: https://docs.google.com/document/d/1CuQPuABMNaXDSIPw4cpNjMeDj__SKqdHKA7Oacvpgog/edit
5pm_4_doc: https://docs.google.com/document/d/1-wbyIuOw5weCJuAxjp6chOp27wqYBDcR8N1W79a3aNw/edit
6pm_1_doc: https://docs.google.com/document/d/1XGotn_g1bG4F9E5d6unJxIyz3PYXufES7yfIHemQusY/edit
6pm_2_doc: https://docs.google.com/document/d/1kN6ONUKWpORFm7wsbSRoeUeaEZwffPqyzldD1TRp2eg/edit
6pm_3_doc: https://docs.google.com/document/d/1USoM6fzZ0dkp9phx0QbQbjauPI5Cr_i3QbDZHpaMAqA/edit
6pm_4_doc: https://docs.google.com/document/d/1xvKiEW0iksVgN_L1qXiD8jrjH9PB16dKEGgUnM4TJQM/edit?usp=sharing
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
* In teams: ~2:30-3:15
  * See separate sections for Courses vs. Happy Cows below.
  
# Product Owner / Product Manager

We'll start today with a presentation by TA Kevin Heffernan about the Product Manager/Product Owner role in a software development team.

The short version is that a product owner is the "voice of the customer" on the team. 
* Why is this important to you?
* Because more and more software engineers required to work on product with more organizations becoming decentralized.

The Product Manager/Owner is part of a team that may also include:
* Developers (folks that actually write the code)
* UX Designers
* QA Engineers

I'll give you an quick overview of what a Product manager/owner does, and then briefly describe how they interact with developers, UX designers and QA engineers.

Practices Vary:
* Note that on some teams, folks may formally be assigned these specific roles
* On others, team members may step in/out of these various roles as needed.

Product Managers/Owners:
* Talk to customers, prospective customers, and end users about their needs
  - These are not necessarily the same.
  - The customer is the one that writes the check, that makes the buy/no-buy decision.
  - The end user is the person that actually uses the software.
* Work with the software development team to turn customer needs into "user stories" 
* The Product Manager may also work with a User Experience (UX) Designer
  * They may also create a storyboard of the sequence of steps a user does to acheive a task
  * The UX Designer may creates mockups of the user interface
  * They may run these mockups by customers
  * They may also conduct User Studies: observing customers using the current interface to see how well the interface works.
* The user stories and UX designs are then turned into issues (aka cards on a Kanban board.)
  * Another 

Kevin will tell you more: [Slides](https://docs.google.com/presentation/d/1Q93KdwjsbL-86Vj2bXWsT1OHDV5UM-d0/edit?usp=sharing&ouid=115856948234298493496&rtpof=true&sd=true)

# Let's do some product ownerish stuff

What we are doing: spending some time thinking about how to design a web application

Why we are doing this: 
* Learning/Educational reasons:
  * Product design is an important skill
  * Good sw dev organizations involve developers in product design
* Practical reasons
  * We are doing a fresh start implementation of both projects (Courses and HappyCows)
  * Reason: we've found a much cleaner/simpler architecture; easier to learn, easier to add new features
  * You'll see this if you compare the code structure of the older controllers and React components from the 
    S21 version of Courses with the structure of the code from W22.
    
    
## First Exercise: Thinking like an end user

There are two versions of this exercise.  Please **_click the triangle_** (▶) to open up the one that pertains to your team.

| Section            | Team 1 | Team 2 | Team 3 | Team 4 |
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
|-------------|-------------|--------|--------|
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

* Please open the Google Document Folder that was shared in the announcement Slack channel. Navigate to your team's document.
* Add a new document with the title `Product Owner Activity, s22-xpm-y 05/10` (put in your team name in place of s22-xpm-y).
* Also put `Product Owner Activity, s22-xpm-y 05/10` as a heading at the top of the text of the document (put in your team name in place of s22-xpm-y).
* Now, add six headers for each of the names of members of your team, so that you each have a section of the document to enter some notes, e.g. 

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

## Step 2: As an individual explore the application 

Then, as individuals, spend 5-10 minutes doing this:

Next: Open up the application.   
* Spend a few minutes exploring the <https://proj-ucsb-courses-search.herokuapp.com> application and it's features. 
* Compare/contrast with <https://my.sa.ucsb.edu/public/curriculum/coursesearch.aspx> and GOLD
* Think about what would be valuable to you as a student.

Finally, also open up the app you are inheriting from the W22 section, here:
 
| W22 Section | S22 Section | Heroku | GitHub |
|-------------|-------------|--------|--------|
| 5pm | 4pm | <https://courses-w22-5.herokuapp.com/> |  <https://github.com/ucsb-cs156-w22/team04-w22-5pm-courses>  |
| 6pm | 5pm | <https://courses-w22-6.herokuapp.com/> |  <https://github.com/ucsb-cs156-w22/team04-w22-6pm-courses>  |
| 7pm | 6pm | <https://courses-w22-7.herokuapp.com/> |  <https://github.com/ucsb-cs156-w22/team04-w22-7pm-courses>  |
{:.table .table-sm .table-striped .table-bordered}

## Step 3: As an individual make some notes 

Then, make some notes about what you see that is good, and what could be improved. Aim for 3 items. 

As you make notes, consider including screenshots.

* What features do you find the most valuable?
* What changes would you make to the user interface?
* What features are missing that you think would be valuable?

If you'd like to see a certain feature, consider mocking up a design of what the forms would look like.

If you'd like to see changes to a User Interface, consider making a screen shot, and then marking it up with
the changes you'd like to see.

## Step 4: With a partner, share your ideas 

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
 
# Step 1: Login to your team's OG Happy Cows deployment.
 
You've been playing HappyCows at the production deployment available from the credentials in [this Slack message](https://ucsb-cs156-s22.slack.com/archives/C03AF7TU1J7/p1649284814753109) and you can continue to play the game there, and learn about it.
 
But the deployment at the `chem123` server does not give you admin access.
 
Your team has its own deployment of the original Happy Cows code (written in Express/Node), at one of the links below; for these deployments,
you *can* give each team member admin access.  This allows you to create new commons, as well as manipulate the parameters of each commons.
 
But to set up admin access,  *each team member first must login to the game* at the link below (select the appropriate link for your team.)
 
**So please login now, at the appropriate link below**.  Just logging in is all you need to do for now.  

Once you've logged in, make a Slack post in your team's channel indicating:
* `I've logged in to the og HappyCows app for this team`  
 
Then go to the next step.
 
 
| S22 Section | Team 3 | Team 4|
|-------------|--------|-------|
| 4pm |  <https://happycows-og-4pm-3.herokuapp.com/> | <https://happycows-og-4pm-4.herokuapp.com/> |
| 5pm |  <https://happycows-og-5pm-3.herokuapp.com/> | <https://happycows-og-5pm-4.herokuapp.com/> |
| 6pm |  <https://happycows-og-6pm-3.herokuapp.com/> | <https://happycows-og-6pm-4.herokuapp.com/> |
{:.table .table-sm .table-striped .table-bordered}

## Step 2: Find your Heroku Deployment
 
You should also find a Heroku Dashboard link for these.  Your team members should have access to these links; make sure that you do.  If any member of your team is missing, add them.
 
| S22 Section | Team 3 | Team 4|
|-------------|--------|-------|
| 4pm |  [Heroku Dashboard Access](https://dashboard.heroku.com/apps/happycows-og-4pm-3/access) | [Heroku Dashboard Access](https://dashboard.heroku.com/apps/happycows-og-4pm-4/access) | 
| 5pm |  [Heroku Dashboard Access](https://dashboard.heroku.com/apps/happycows-og-5pm-3/access) | [Heroku Dashboard Access](https://dashboard.heroku.com/apps/happycows-og-5pm-4/access) | 
| 6pm |  [Heroku Dashboard Access](https://dashboard.heroku.com/apps/happycows-og-6pm-3/access) | [Heroku Dashboard Access](https://dashboard.heroku.com/apps/happycows-og-6pm-4/access) | 
{:.table .table-sm .table-striped .table-bordered}
  
## Step 3:  Giving each member of your team admin access to the app.

Once each team member has logged in to your Happy Cows og app, you can give everyone admin access. This involved a manual change to the SQL database.
 
For this, step, it is easiest to do this at the CSIL prompt, because the
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
 
## Step 4: Test the admin access 

At this point, every member of your team should have admin access.  You can test this by visiting the url `/admin` on your site, e.g.

| S22 Section | Team 3 | Team 4|
|-------------|--------|-------|
| 4pm |  <https://happycows-og-4pm-3.herokuapp.com/admin> | <https://happycows-og-4pm-4.herokuapp.com/admin> |
| 5pm |  <https://happycows-og-5pm-3.herokuapp.com/admin> | <https://happycows-og-5pm-4.herokuapp.com/admin> |
| 6pm |  <https://happycows-og-6pm-3.herokuapp.com/admin> | <https://happycows-og-6pm-4.herokuapp.com/admin> |
{:.table .table-sm .table-striped .table-bordered}

From there, you can experiment with both the admin and user features of the app.

If you get this instead, then it means you were not successfully added as an admin.  Try repeating Steps 1, 2, and 3.

<img width="227" alt="image" src="https://user-images.githubusercontent.com/1119017/167707600-1da74cfd-d697-4d4e-ab65-6e46d0399721.png">

 
## Step 5: Learning about Happy Cows
 
There are four documents that you should read to learn about the HappyCows game.  Please take 5-10 minutes for each team member to look over these documents.
 
1. [Happy cows description: A text description of the game](https://docs.google.com/document/d/1pKpvrSHJ1PKCaSsjNa_xv79u3NzLl6jV/edit?usp=sharing&ouid=115856948234298493496&rtpof=true&sd=true), by Prof. Mattanjah de Vries, the UCSB Chemistry professor that developed the game.
2. [Happy cows intro: A set of slides about the game](https://docs.google.com/presentation/d/1oCZ2ePYW5hy4JkFz8z-2-fz-tBOOy-id/edit?usp=sharing&ouid=115856948234298493496&rtpof=true&sd=true) also by Prof. de Vries.
3. [`gamePlay.md`: A high level description of the game](https://github.com/ucsb-cs156-w22/HappierCows/blob/main/docs/gamePlay.md) by Seth VanBrocklin, who was an LA for CMPSC 156 during W22, and graduated after W22.   (Seth may be available to consult with teams in class.)
4. [`newFeatures.md`: A description of possible future designs for HappyCows](https://github.com/ucsb-cs156-w22/HappierCows/blob/main/docs/newFeatures.md) A description of possible future designs for HappyCows, also written by Seth.
 
 
## Step 6: As a group, organize the document into sections by user

* Please open the Google Document Folder that was shared in the announcement Slack channel. Navigate to your team's document.
* Add a new document with the title `Product Owner Activity, s22-xpm-y 05/10` (put in your team name in place of s22-xpm-y).
* Also put `Product Owner Activity, s22-xpm-y 05/10` as a heading at the top of the text of the document (put in your team name in place of s22-xpm-y).
* Now, add six headers for each of the names of members of your team, so that you each have a section of the document to enter some notes, e.g. 

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

## Step 7: As an individual explore the original application 

Then, as individuals, spend 5-10 minutes doing this:

Next: Open up the older HappyCows application using the Heroku deployment assigned to your team:

| S22 Section | Team 3 | Team 4|
|-------------|--------|-------|
| 4pm |  <https://happycows-og-4pm-3.herokuapp.com/> | <https://happycows-og-4pm-4.herokuapp.com/> |
| 5pm |  <https://happycows-og-5pm-3.herokuapp.com/> | <https://happycows-og-5pm-4.herokuapp.com/> |
| 6pm |  <https://happycows-og-6pm-3.herokuapp.com/> | <https://happycows-og-6pm-4.herokuapp.com/> |
{:.table .table-sm .table-striped .table-bordered}
 
* Spend a few minutes exploring the current Happy Cows application and its features. 
* Think about features that would make it easier for the instructor/admin to set up the game.
* Think about features that make game play more interesting

## Step 8: As an individual explore the W22 application 
 
Then open up the app you are inheriting from the W22 section, here:
 
| S22 Section | W22 Section | Heroku | GitHub |
|-|-|-|-|
| 4pm | 5pm | <https://team04-w22-5pm-happycows.herokuapp.com/> |  <https://github.com/ucsb-cs156-w22/team04-w22-5pm-HappyCows>  |
| 5pm | 6pm | <https://team04-w22-6pm-happycows.herokuapp.com/> |  <https://github.com/ucsb-cs156-w22/team04-w22-6pm-HappyCows>  |
| 6pm | 7pm | <https://team04-w22-7pm-happycows.herokuapp.com/> |  <https://github.com/ucsb-cs156-w22/team04-w22-7pm-HappyCows>  |
{:.table .table-sm .table-striped .table-bordered}
 
See what features work, and what features are missing.  You may also want to consult with the LAs or other staff.
 
It may also be useful to consult the Kanban boards:
 
| S22 Section | W22 Section | Team 3 Kanban board | Team 4 Kanban board |
|-|-|-|-|
| 4pm | 5pm | [w22-5pm-3](https://github.com/ucsb-cs156-w22/team04-w22-5pm-HappyCows/projects/1) | [w22-5pm-4](https://github.com/ucsb-cs156-w22/team04-w22-5pm-HappyCows/projects/2) |
| 5pm | 6pm | [w22-6pm-3](https://github.com/ucsb-cs156-w22/team04-w22-6pm-HappyCows/projects/1) | [w22-6pm-4](https://github.com/ucsb-cs156-w22/team04-w22-6pm-HappyCows/projects/2) |
| 6pm | 7pm | [w22-6pm-7](https://github.com/ucsb-cs156-w22/team04-w22-7pm-HappyCows/projects/1) | [w22-7pm-4](https://github.com/ucsb-cs156-w22/team04-w22-7pm-HappyCows/projects/2) |
{:.table .table-sm .table-striped .table-bordered}
 
 
## Step 9: As an individual make some notes 

Then, make some notes about what you see that is good, and what could be improved. Aim for 3 items. 

As you make notes, consider including screenshots.

* What features do you find the most valuable?
* What changes would you make to the user interface?
* What features are missing that you think would be valuable?

If you'd like to see a certain feature, consider mocking up a design of what the forms would look like.

If you'd like to see changes to a User Interface, consider making a screen shot, and then marking it up with
the changes you'd like to see.

## Step 10: With a partner, share your ideas 

With a partner from your team, discuss some of the ideas you each came up with independently. 

Take turns, half a minute each pitching each other your ideas.

Then, choose your favorite two to share with the team.

## Step 11: As a group, discuss your lists (8 minutes)

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
 
# Step 12: As a class, each team shares 1 or 2 of the ideas your team came up with

We'll come around to allow each group to spend time sharing their idea(s). 

One student (maybe two) from each team will have half a minute to share their idea with the class.

So, keep it short! This is a low presure exercise meant to be fun and not test your public speaking skills. 

At most share 2 ideas that your team felt would be high priority with the class. 


</details>


# What happens next?
 
In a future exercise, we'll talk about User Stories
* [User Stories](https://ucsb-cs156.github.io/topics/user_stories/) `As a __ I can __ so that __`
 
You may be asked to take the high level ideas you came up with in this exercise, and turn them first into **User Stories**, and then into 
**issues on a Kanban board** with [**Acceptance Criteria**](https://ucsb-cs156.github.io/topics/agile_acceptance_criteria/).
  
# Links to Writeups
 
| Section | Team 1 | Team 2 | Team 3 | Team 4 | 
|-|-|-|-|-|
| 4pm | [s22-4pm-1]({{page.4pm_1_doc}}) | [s22-4pm-2]({{page.4pm_2_doc}}) | [s22-4pm-3]({{page.4pm_3_doc}}) | [s22-4pm-4]({{page.4pm_4_doc}}) | 
| 5pm | [s22-5pm-1]({{page.5pm_1_doc}}) | [s22-5pm-2]({{page.5pm_2_doc}}) | [s22-5pm-3]({{page.5pm_3_doc}}) | [s22-5pm-4]({{page.5pm_4_doc}}) | 
| 6pm | [s22-6pm-1]({{page.6pm_1_doc}}) | [s22-6pm-2]({{page.6pm_2_doc}}) | [s22-6pm-3]({{page.6pm_3_doc}}) | [s22-6pm-4]({{page.6pm_4_doc}}) | 
{:.table .table-sm .table-striped .table-bordered}

