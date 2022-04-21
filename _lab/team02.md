---
desc: "Team Project: Spring Boot Backend, part 2 (authenticated CRUD)"
assigned: 2022-04-21 14:00
due: 2022-04-29 23:59
github_org: ucsb-cs156-s22
layout: lab
num: team02
ready: false
---

{% include drop_down_style.html %}


# NOT READY
# DON'T START YET
# NOT READY
# DON'T START YET
# NOT READY
# DON'T START YET
# NOT READY
# DON'T START YET
# NOT READY
# DON'T START YET
# NOT READY
# DON'T START YET
# NOT READY
# DON'T START YET
# NOT READY
# DON'T START YET
# NOT READY
# DON'T START YET
# NOT READY
# DON'T START YET
# NOT READY
# DON'T START YET
# NOT READY
# DON'T START YET

In this team project, our starter code has a  frontend and backend, however we are still focusing only on the backend part.  The front end provides only
a place for us to login with our Google account.

We are focusing on learning these new Spring Boot backend concepts:

* Creating SQL database tables using `@Entity` and `@Repository`
* Using the Lombok annotations: `@Data`, `@NoArgsConstructor`, `@Builder`, etc.
* Implementing controller routes for CRUD operations (Created, Read, Update, Destroy)
* Writing unit tests for controller CRUD operations, including the use of:
  - Spring `MockMvc`
  - Mockito methods for creating mocks of repositories and services (`when`, `verify)
  - the idea of "dependency injection"

In addition, we'll practice further with a few concepts that we touched on in `jpa03`, but may not have fully fleshed out:
- Set up of the documentation repos, the `-docs` and `-docs-qa` repos
- Working with feature branches, issues, a Kanban board, pull requests, and GitHub actions scripts
- Working with code coverage and mutation testing

## The starting code

Your starter code provides Spring Boot code with the ability to do CRUD operations on two database tables:

* UCSBDates
* UCSBDiningCommons

These tables are set up to match the data that is available through two public APIs that are provided by UCSB and documented at
<https://developer.ucsb.edu>.

The `UCSBDates` tables has three columns, and is intended to store data like that shown here:


The `UCSBDiningCommons` table has six columns, and is intended to store data like that shown here:


## Working with Swagger 



## Your task: add CRUD for additional database tables


You'll be adding CRUD operations for six additional database tables; one per team member:

Here are the tables you'll be adding:

### UCSB Dining Commons Menu item


<details>
<summary>
For details on the UCSB Dining Commons Menu item, click the triangle
</summary>

The `UCSBDiningCommonsMenuItem` will use a `Long` as it's `id` field, and will have these additional columns:

* `String diningCommonsCode`
* `String name`
* `String station`

Here are some sample values:

| id | diningCommonsCode | name | station |
|----|-------------------|------|---------|
| 1  | ortega            | Baked Pesto Pasta with Chicken | Entree Specials |
| 2  | ortega            | Tofu Banh Mi Sandwich (v)  | Entree Specials |
| 3  | ortega            | Chicken Caesar Salad  | Entrees |
| 5  | portola            | Cream of Broccoli Soup (v) | Greens & Grains |

</details>  
  
### UCSB Organization

<details>
<summary>
For details on the UCSB Organization item click the triangle
</summary>


The `UCSBOrganization` table will use the `orgCode` field (a String) as it's id field, and will have these columns:

* String orgCode
* String orgTranslationShort
* String orgTranslation
* boolean inactive

Here are some sample values:

| orgCode | orgTranslationShort | orgTranslation | inactive |
|----|-------------------|------|---------|
| ZPR | ZETA PHI RHO | ZETA PHI RHO | false |
| SKY | SKYDIVING CLUB | SKYDIVING CLUB AT UCSB | false |
| OSLI | STUDENT LIFE | OFFICE OF STUDENT LIFE | false |
| KRC | KOREAN RADIO CL | KOREAN RADIO CLUB | false |

</details>
  
## What you'll do: Process

From a process standpoint, this project works the same as team01:


Here's how that will play out in detail:
1. To start, each of you should clone your team's `team02-teamname` repo, which should already have a Kanban board set up for it.
2. On the team's Kanban board, there should be three types of issues, marked with Tags
   - Set up tasks: done at the start of the project
   - Coding tasks: done in the middle of the project
   - Clean up tasks: done at the end of the project
   Notice the tags for each of these types of issues.
3. First, divide up the set up tasks among the members of the team, and assign each of those to a team member.   Leave them in the "to do" column, though, until you actually start working on the issue.
4. Then, divide up the six database tables among the team members.  I suggest that you do this on your team slack channel in a single post, and then "pin" that post to your channel.
   That post might look something like this:

   ```
   Adam: 
   Brianna:
   Chris:
   Danny:
   Erin:
   Fay:
   ```
   Each one should be assigned to a specific team member.  You'll see that for each of the database 
   tables, there are five issues:
   * create_database_table
   * add_list_all_and_post_endpoints
   * add get for single item
   * add put for single item
   * add delete for single item 

   You should 
7. Next, you'll create a Kanban board with columns: `Todo`, `In Progress`, `In Review`, `Done`
8. You'll then populate the `Todo` column with a set of tasks, which are called *Issues* in the GitHub implementation of Kanban.
9. You'll then assign those tasks to members of the team, moving them into the "In Progress" as each task is assigned.  
   - You may assign tasks either to individuals, pairs, or even larger groups (so-called "mobs", as in [*Mob Programming*](https://en.wikipedia.org/wiki/Mob_programming))
   - But be sure that if you assign a task to more than one person, that each member of the pair or mob is legitimately committed to contributing to working on the task, and committed to getting it finished.
10. Once a pull request is complete for a given task, you move it into the `In Review` column
   - At this stage, you seek a code review from a member of the team that was not involved in the coding.
   - If it was a true "all-team mob", than it's fine to get a code review from someone that participated, but this is rare.
   - Also, at this stage, if the PR is not "green on CI", meaning that all of the GitHub actions scripts show green checks, this is when you 
     should address that, before merging the pull request.
6. Only when the PR is merged does the issue get moved into the done column.

## What you'll do: Content/Product

From a high-level standpoint, you'll be doing these things:

Set up Tasks:

* Setting up a Repo with qa and prod deployments on Heroku
* Configuring the documentation repos
* Configuring Codecov

Coding Tasks:
* Adding database tables for University Subreddits, UCSB Subjects, and UCSB Requirements
* Setting up CRUD operations for all three of those tables
* Adding backend test coverage for all of that

In the next assignment, we'll turn to the front end, and put a front end for CRUD operations on 
all three of those tables.

# Getting started

To get started:

* One member of your team should clone your teams empty team02 repo
* Add the STARTER-team02 repo as a remote called starter
* Do `git checkout -b main`, `git pull starter main`, `git push origin main`

Then, you'll manually run a GitHub workflow to populate a Kanban board with issues.  Here's what that looks like.

First, you need to go to the Actions tab:

<img alt="" src="https://user-images.githubusercontent.com/1119017/151859324-1c46cd9b-f7c0-4917-a98e-6cf685ba3519.png" width="600" />



Click the button to enable actions. 

Next you'll see this list of actions. You want to select "Create Issue from File"

<img alt="" src="https://user-images.githubusercontent.com/1119017/151859445-177a317a-2d11-41d1-9c4e-b5adf1f22a13.png" width="200" />

You'll then see that this action can be triggered manually.  Click `Run Workflow` to trigger the action:

<img alt="" src="https://user-images.githubusercontent.com/1119017/151859553-e6940d7e-0ee3-4e0e-888c-b48af6568482.png" width="600" />


You'll see that the workflow is running:

<img alt="" src="https://user-images.githubusercontent.com/1119017/151859733-e8e05c83-2426-4463-8bba-90ca974dd9ad.png" width="600" />


As it runs, issues will appear under the issues tab, and a project will appear under the project tab.  When completed, you
should have 1 Project (i.e. a Kanban board), and 18 issues:

<img alt="" src="https://user-images.githubusercontent.com/1119017/151859918-20c23329-ccf7-4a79-a75b-d0e815a0377a.png" width="600" />

Next, go to the Projects tab, and view your Kanban board; to find it you'll need to bypass the new Projects Beta, and go
to the old Projects interface.  It's the place that says "Projects 1" in the left navigation:

<img alt="" src="https://user-images.githubusercontent.com/1119017/151860027-1c696786-8e31-4766-ab7c-7f4effd8ef5c.png" width="600" />


There you should see a project called `Team02`.  Click on that:

<img alt="" src="https://user-images.githubusercontent.com/1119017/151860130-ceebc42a-2782-4909-a153-e6a5205e68d6.png" width="600" />

This, finally is your Kanban board:

<img alt="" src="https://user-images.githubusercontent.com/1119017/151860181-7ce6b97a-4383-4e2f-a14e-7aa653fe6dd6.png" width="600" />


Click to add three new columns.  The first is called "In Progress"

<img alt="" src="https://user-images.githubusercontent.com/1119017/151860236-a053eb68-d811-4d09-b715-c63d5d4ef0a5.png" width="600" />

<img alt="" src="https://user-images.githubusercontent.com/1119017/151860278-240dc265-ea4e-4aee-b0e0-3648437301fa.png" width="600" />

Then, add columns for "In Review" and "Done" to the right:


<img alt="Four columns" src="https://user-images.githubusercontent.com/1119017/151860348-a7d64d66-93f8-4969-b6a5-4c28e3b90a67.png" width="800" />

### Implement CRUD operations for a database table

We'll start with the example of adding a table for University Subreddits

In team01, one of the endpoints served up an API for looking up a list of University Subreddits by reading a CSV file from a GitHub repo on the web, parsing it, and serving it up in JSON. 

It used the code in the java file [`CollegeSubredditQueryService`](https://github.com/ucsb-cs156-w22/STARTER-TEAM01/blob/main/src/main/java/edu/ucsb/cs156/spring/backenddemo/services/CollegeSubredditQueryService.java) to accomplish this.
 
However, the implementation of this service, while relatively simple, uses a rather inefficient appraoch. In particular, each call to this service:
* does a backend call to do a GET request relatively static CSV file in a GitHub repo with a CSV file of College Subreddits, [`karlding/college-subreddits`](https://github.com/karlding/college-subreddits), namely the file [`colleges.csv`](https://raw.githubusercontent.com/karlding/college-subreddits/master/data/colleges.csv)
* parses the CSV
* converts the entire thing to JSON and then returns it

Given how slowly this data changes, it seems more effici`ent to load this data once, and then serve it up on subsequent requests.  

For this, we can use an SQL database table.  
* This allows us to load the data just once, on a server that is likely co-located with our running app (i.e. in the same data center)
* It also allows us to index the collection of data, and search efficiently by school name, location, or subreddit name
* Finally, it gives us the ability to efficiently create, read, update and destroy additional records in the data 
  (without having to wait for a pull request to the [`karlding/college-subreddits`](https://github.com/karlding/college-subreddits) repo.

If you haven't worked with SQL database tables before, think of each database table as if it is a spreadsheet with rows and columns.
* The columns in our table will be: `name`,`location`,`subreddit`. 
* In addition, while it is not absolutely required, it is typical and usually helpful to add an `id` column to each table: the `id` is an arbitrary integer value that identifies each row in the table.
* The rows are the individual data records

So, for example, the table might look like this:

| id | name | location | subreddit |
|-|-|-|-|
|1 |Aberystwyth University | Aberystwyth, Wales, United Kingdom | Aberystwyth |
|2|Acadia University | Wolfville, Nova Scotia, Canada | AcadiaU |
|3|Algonquin College | Ottawa, Ontario, Canada | Algonquin_College |
|4|Amarillo College | Amarillo, Texas, United States| amarillocollege |
{:.table .table-sm .table-striped .table-bordered}

Note that while the `id` values start out from `1` and are consecutive integers, if we were to delete row `2` and then readd it to the table, the resulting table would look like this; numbers typically don't get reused.  


| id | name | location | subreddit |
|-|-|-|-|
|1 |Aberystwyth University | Aberystwyth, Wales, United Kingdom | Aberystwyth |
|3|Algonquin College | Ottawa, Ontario, Canada | Algonquin_College |
|4|Amarillo College | Amarillo, Texas, United States| amarillocollege |
|5|Acadia University | Wolfville, Nova Scotia, Canada | AcadiaU |
{:.table .table-sm .table-striped .table-bordered}

As an aside: you may wonder what happens when we run out of numbers.  Since these `id` numbers are typically stored in a 64-bit Java `Long`, the maximum number is: `9,223,372,036,854,775,807L`.   
* If you stored 1 Million records per second, 24 hours a day, 7 days a week, it would take you [292 thousand years](https://www.google.com/search?q=9%2C223%2C372%2C036%2C854%2C775%2C807+%2F+1000000+%2F+60+%2F+60+%2F+24+%2F+365&rlz=1C5CHFA_enUS888US889&sxsrf=APq-WBtGUMS1ceirZg3u9OrjxeaktzoWaw%3A1643567397963&ei=Jdn2Yen0Oc3EkPIP3du9gA4&ved=0ahUKEwipm63Xjdr1AhVNIkQIHd1tD-AQ4dUDCA4&uact=5&oq=9%2C223%2C372%2C036%2C854%2C775%2C807+%2F+1000000+%2F+60+%2F+60+%2F+24+%2F+365&gs_lcp=Cgdnd3Mtd2l6EANKBAhBGAFKBAhGGABQ4w1Y9A9gxxZoAXAAeACAAZcBiAGYA5IBAzAuM5gBAKABAcABAQ&sclient=gws-wiz) to cycle through this many id numbers.  
* That's also over 18,000 records for every square meter on the face of the planet earth.  Not sure what database table needs that many records.

To add an SQL database table in Spring Boot, you typically add two files:

* A Java class that is annotated with `@Entity`; each instance of this class represents a single row in the database table
* A Java class that is annotated with `@Repository`; each instance of this class represents a database table.

There is more information in the issues on the Kanban board to guide you through the rest of the process.

# More Hints

We may add more hints about working with the team02 code as we discover what
problems studnets run into.

In the meantime, use the 

# A note about open source

Note that this assignment is open source.

The repos are public *on purpose*.
* You are encouraged to consult with one another within and across teams where it helps
  your learning.
* That does not mean that you can cheat by just copying code from another team.
* You are *not* permitted to just look at another team's code, even though you "can".
* It does mean that you should try to solve the problems as best you can, but you may 
  consult with members of other teams as you work.  In that context, you may look at 
  other team's code.

This isn't hard.   You all *know* when you are are looking at other team's work to
try to learn, versus when you are just looking at it as a shortcut to learning.

I'm trusting you to do the right thing.   This is practice for when, later on, you are
all working on different assignments.


# Clarifications

## For the issue "Set up docs"

Note that step 1 says: 

> Make a new branch `xy-setup-docs` where `xy` are your intials.

To clarify: that is a new branch on yoru team02 repo, not the team02-docs or team02-docs-qa repos.

The same goes for pretty much all of the instructions: you are editing the team repo.
