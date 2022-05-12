---
desc: "Team Project: FrontEnd CRUD, part 1: Index Page, and Delete Column"
assigned: 2022-05-12 14:00
due: 2022-05-18 23:59
github_org: ucsb-cs156-s22
layout: lab
num: team03
ready: false
gauchospace_url: update_this_url
---

{% include drop_down_style.html %}


# NOT READY YET
# NOT READY YET
# NOT READY YET
# NOT READY YET
# NOT READY YET
# NOT READY YET
# NOT READY YET
# NOT READY YET


## Big Picture: what is team03 all about?

From a high-level standpoint, you'll be doing these things:

Set up Tasks:

* Setting up qa and prod deployments on Heroku 
  - If your team02 is graded, you may reuse your team02 heroku deployment
  - No need to rename it; just deploy the new code base to it
  - This will save you time, since you wont have to update the Google OAuth secrets
* Configuring the `-docs` and `-qa` repos
  - You will need to do this, and it will actually matter, since we'll be using storybook
* Configuring Codecov
* Setting up your own Kanban board
  - In this project, you'll create a Kanban board from scratch
  - You'll also be responsible for creating your own issues, and adding the acceptance criteria

Coding Tasks:
* Adding the index page and table components for each of your six database tables
* Adding testing for these

In team04, we'll add the create and edit functions as well.  For team03, you'll continue to do create and edit through the Swagger end point directly.

For this assignment, we are still dealing directly with the backend via Swagger.

# Setting up your Kanban board

One team member should take on the task of setting up the Kanban board.  Decide who will do that, and document that decision on your Slack channel.


If you go on the slack channel and no one from your team has done it yet, it might as well be you!  It's super easy.

To learn how, **_click the triangle_** (▶) to reveal the steps.

<details>
<summary>
Creating your own Kanban board
</summary>

1. Tell the rest of the team (via your Slack channel) that you are setting up the Kanban board.

2. Go to your team03 repo.  At this stage, it doesn't matter whether it's still empty, or whether it already has stuff in it.

   | Section | 1 | 2| 3| 4| 
   |-|-|-|-|-|
   | 4pm | [team03-s22-4pm-1](https://github.com/ucsb-cs156-s22/team03-s22-4pm-1) | [team03-s22-4pm-2](https://github.com/ucsb-cs156-s22/team03-s22-4pm-2)    | [team03-s22-4pm-3](https://github.com/ucsb-cs156-s22/team03-s22-4pm-3) | [team03-s22-4pm-4](https://github.com/ucsb-cs156-s22/team03-s22-4pm-4) | 
   | 5pm | [team03-s22-5pm-1](https://github.com/ucsb-cs156-s22/team03-s22-5pm-1) | [team03-s22-5pm-2](https://github.com/ucsb-cs156-s22/team03-s22-5pm-2)    | [team03-s22-5pm-3](https://github.com/ucsb-cs156-s22/team03-s22-5pm-3) | [team03-s22-5pm-4](https://github.com/ucsb-cs156-s22/team03-s22-5pm-4) | 
   | 6pm | [team03-s22-6pm-1](https://github.com/ucsb-cs156-s22/team03-s22-6pm-1) | [team03-s22-6pm-2](https://github.com/ucsb-cs156-s22/team03-s22-6pm-2)    | [team03-s22-6pm-3](https://github.com/ucsb-cs156-s22/team03-s22-6pm-3) | [team03-s22-6pm-4](https://github.com/ucsb-cs156-s22/team03-s22-6pm-4) | 
   {:.table .table-sm .table-striped .table-bordered}

3. Click on the Projects tab. It should look like this:

   <img width="593" alt="image" src="https://user-images.githubusercontent.com/1119017/167972688-04403c2b-65cf-4790-9a22-b7e8bc850061.png">

4. Click on the bottom `Projects` button (not the `Beta` one, but the other one). Your screen should then look like this:

   <img width="1183" alt="image" src="https://user-images.githubusercontent.com/1119017/167972869-361f8df9-3d0b-4ede-bf38-df3fee636135.png">

5. Click the green `New Project` button, at upper right.  Your screen should then look like this:

   <img width="990" alt="image" src="https://user-images.githubusercontent.com/1119017/167972920-a8a0eb57-102e-43d1-baa6-f3cf2e964b2d.png">

6. Fill in the project name with your team name (e.g. `s22-4pm-1`).  You can leave the description blank. Then select `Automated Kanban with Reviews` from the dropdown menu (as shown), and finally click the `Create Project` button.
   <img width="472" alt="image" src="https://user-images.githubusercontent.com/1119017/167973020-b9d862b4-3dc9-4110-8da5-6afb145a15b4.png">

7. In the `To Do` column, you'll now have some annoying starter cards, as shown below.  Click in the three dots at upper right on
   each of them to get rid of them, so that you have an empty board:

   <img width="438" alt="image" src="https://user-images.githubusercontent.com/1119017/167973169-b79f2879-cab8-4f2e-8f8d-ace42d1675cf.png">

   When done, it should look like this:

   <img width="1720" alt="image" src="https://user-images.githubusercontent.com/1119017/167973263-66ee283e-7289-4d6d-8ac0-491cf367343c.png">

8. Congratulations: your team can now start adding issues to your Kanban board.

</details>
  
# Adding Issues

Now, each of you may choose to continue working on the same database table that you did in team02, or you can choose to mix it up; that's a decision I'll leave up to the team.

As a reminder, these are the six tables:

* Menu Item
* Organizaton
* Recommendation
* Review
* Help Request
* Article

Choose which of these you are going to work on.  Then, for your database table, you are going to add a few issues to the Kanban board.

The easiest way to do this is to start by creating *Cards* on the Kanban board, and then *Converting them to Issues*.

Here is what that process looks like:

![create-card-convert-to-issue](https://user-images.githubusercontent.com/1119017/167974490-12699832-a56b-4e41-9ac5-cca96f31c1a3.gif)

Here are the cards you need to create.  I'm using `Recommendation` as the example here; substitute in your database table name in place of that.

* Add Recommendation menu to nav bar
* Add Placeholder for Recommendation Index Page
* Add RecommendationTable component to Storybook (along with fixtures)
  - Note that you can include the DeleteColumn at this stage, or not; your choice.
* Replace RecommendationTable placeholder page with one that includes Recommendation Table
* Add Delete Column to RecommendationTable (if not already done)

The idea is that you should *make a separate pull request* for each of these issues; and it should be code reviewed and merged separately.

For each, you should get all of the tests to pass before moving on to the next issue. 
* You may find this annoying at first, and you may think that it will slow you down.
* That may be true when you are working as an individual
* But keep in mind: up until now, and still including this team project, the tasks are designed so that you stay out of each other's way.
* When it comes to the real project, you'll constantly be in each other's way, unless you work in *very small pieces*, adding the test
  coverage *as you go*.
* This exercise is designed to help you develop that skill.

Once you've made the cards and converted them to issues, the next step is to add detail to each issue, including acceptance criteria.

# Adding the acceptance criteria

To add acceptance criteria, you need to go to the full issue view.  Here's how that looks:

# More details on team03

In this team project, our starter code has a frontend and backend, and we are focusing only on the frontend; you will likely not have to make any modifications to the backend.

We are focusing on learning these new React concepts:

* Adding new items to the navbar
* Adding components for new placeholder pages
* Adding routes in `App.js` to link urls to pages
* Creating a component that uses the `OurTable` component to create a table
* Changing the placeholder page so that it loads data using the `useBackend` hook to fetch data
* Using the `ButtonColumn` feature of `OurTable` to add a delete button 
* Using `npm test` to run unit tests
* Using `npm run coverage` to run test coverage
* Using `npx stryker run` to run mutation coverage
* Using `npm run storybook` to visualize frontend components in isolation
 

## Copying your team02 work into the starter code.

You'll start with the starter code `STARTER-team03`, and then add to it the files you created in team02 to implement
the database tables and backend CRUD operations

These will likely include, for each of the database tables you created in team02:
* A Java class for the `@Entity`
* A Java class for the `@Repository`
* A Java class for the Controller
* A Java class containing Controller tests

The first pull request you make should simply copy those files from your team02 repo into the appropriate directories.


## Your next task: add a menu with one option for each of the six database tables

You'll see on the menu bar that there are menus for Todos, Dining Commons and Dates.

You should add a menu item similar to that for Dining Commons, for the database table you are working on.

* Menu Item
* Organizaton
* Recommendation
* Review
* Help Request
* Article

You'll need to coordinate with your teammates to ensure that you don't end up with merge conflicts.

It may be easier to have one person on the team add all six menu items; that's up to you to coordinate.

## Next Steps

Just as shown in the video from Thursday May 5:

* You'll first add a placeholder for your index page.
* Then you'll make sure that the menu item links to that placeholder page.
* Not show in that video, but shown in an upcoming video, you'll need to add test coverage

This is a good place to do a pull request.

Then:
* Add the delete column, and get that working
* Add tests for that
* Do another pull request

When that's done, you are finished with your part for team03.

# Check in with the team

* See if there are code reviews that you can help with
* See if anyone else on the team needs help with their tasks

# Your next steps

The team03 assignment will be followed shortly by team04, which will use the same repo and code base, and kanban board; you can think of it as
"team03 part 2".

In team04, you'll add a data entry form for each of your six database records.   That data entry form will be used for both entering new records (i.e. the POST route)
as well as editing database records (the PUT) route.   You'll also add Create and Edit pages to the pages directory.

You'll then hook up the "edit column" in the table to the Edit page.   That's coming soon.

# Asking for help

  
If you need additional guidance, ask on the `#help-team03` channel, and we'll try to steer you in the right direction.

# When you are done

When all branches are merged to main, all tasks on Kanban board in the done column, please submit on [Gauchospace]({{page.gauchospace_url}})
