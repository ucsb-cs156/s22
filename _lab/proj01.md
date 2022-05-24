---
desc: "Team Legacy Code Project"
assigned: 2022-05-12 14:00
due: 2022-06-01 23:59
github_org: ucsb-cs156-s22
layout: lab
num: proj01
ready: true
gauchospace_url: https://gauchospace.ucsb.edu/courses/mod/assign/view.php?id=2038491&forceview=1
starter_courses: git@github.com:ucsb-cs156-s22/STARTER-courses-search.git
starter_cows: git@github.com:ucsb-cs156-s22/STARTER-happycows.git
---

These are the instructions for the legacy code project phase of the course.

Everything up until now has been a kind of "warm up" for this.  This is when you work on a project that:
* has "real users" 
* has a code base that was worked on by students before this quarter (specifically during W22)
* has a code based that will continue to be worked on by students next time the class is offered (specifically during F22)

There will be six groups, each composed of two teams:

| Group | Teams | Project |
|-------|-------|---------|
| 4pm-courses   | s22-4pm-1, s22-4pm-2 | Courses    | 
| 4pm-happycows | s22-4pm-3, s22-4pm-4 | Happy Cows | 
| 5pm-courses   | s22-5pm-1, s22-5pm-2 | Courses    | 
| 5pm-happycows | s22-5pm-3, s22-5pm-4 | Happy Cows | 
| 6pm-courses   | s22-6pm-1, s22-6pm-2 | Courses    | 
| 6pm-happycows | s22-6pm-3, s22-6pm-4 | Happy Cows | 
{:.table .table-sm .table-striped .table-bordered}


# High Level Plan

| Teams | Project | Epic | Starter Code  |
|-------|---------|------|---------------|
| 4pm-1, 5pm-1, 6pm-1 | Courses Search | TBD | <https://github.com/ucsb-cs156-s22/STARTER-courses-search> |
| 4pm-2, 5pm-2, 6pm-2 | Courses Search | TBD | <https://github.com/ucsb-cs156-s22/STARTER-courses-search> |
| 4pm-3, 5pm-3, 6pm-3 | Happy Cows | TBD | <https://github.com/ucsb-cs156-s22/STARTER-happycows> |
| 4pm-4, 5pm-4, 6pm-4 | Happy Cows | TBD | <https://github.com/ucsb-cs156-s22/STARTER-happycows> |
{:.table .table-sm .table-striped .table-bordered}


## Epics

You'll find an overview of what to do in each Epic here; note however, that this is a high-level document, and is subject to
negotiation.  You should talk with the other team you are paired with to make sure you are not duplicating effort, or going in different directions, and that your code will all work together.

You are ultimately evaluated separately, but you are evaluated in part on how well you cooperated with your partner team, and worked for the greater good of both teams.

We have set up repos for each of the teams.  Note that teams work in pairs in the same repo:

| Team | Team | Repo |
|------|------|------|
| s22-4pm-1 | s22-4pm-2 | <https://github.com/ucsb-cs156-s22/s22-4pm-courses> |
| s22-4pm-3 | s22-4pm-4 | <https://github.com/ucsb-cs156-s22/s22-4pm-happycows> |
| s22-5pm-1 | s22-5pm-2 | <https://github.com/ucsb-cs156-s22/s22-5pm-courses> |
| s22-5pm-3 | s22-5pm-4 | <https://github.com/ucsb-cs156-s22/s22-5pm-happycows> |
| s22-6pm-1 | s22-6pm-2 | <https://github.com/ucsb-cs156-s22/s22-6pm-courses> |
| s22-6pm-3 | s22-6pm-4 | <https://github.com/ucsb-cs156-s22/s22-6pm-happycows> |
{:.table .table-sm .table-striped .table-bordered}

You will NOT be able to merge your own pull requests in these repos. Instead:
* You need to get the PR to be fully green on CI/CD (i.e. all GitHub actions scripts passing)
* You need to get at least one approved code review from a fellow team member that did not work on the story
* You need to a get a *code review from a staff member*
* The staff member will then merge the PR, *and award points to your team*.

Your team should try  to accumulate 100 points to get full credit (you may go up to 110 for extra credit.)

If you only accumulate 90, that's an A-, 83 is a B, etc.


# Setup Tasks

There are a group of setup tasks that need to be done for both projects.

Then there are a few setup tasks that are specific to each project.

First, the general ones.  

The first task is to set up a Kanban board for your team.  Assign one person on your team to do this, and note who that will be in your Slack channel. Note that two teams are working together in a group: e.g. 4pm-1 and 4pm-2 are two separate teams in a group.  You should set up a separate Kanban board for 4pm-1 and 4pm-2, not a single one for the entire group.  (There are pros/cons to each approach, but this is the way we are proceeding.)

Once the Kanban board is setup, you may use it to track these additional tasks:

* Someone on the -1 or -3 team for each repo should make an issue, branch and PR to add the -docs and -docs-qa links to the `README.md` file of your group's shared repo.   
  - As part of this issue, set up the DOCS_TOKEN for the repo.
  - Test that the GitHub Actions for publishing the docs to both -docs and -docs-qa work properly; that should be one of the
    acceptance criteria for the issue.
  - When merged this will be worth 5 points for that team.
* Someone on the -2 or -4 team for each repo should make a production deployment of the repo that has the same name as the repo (e.g. <https://s22-5pm-happycows.herokuapp.com>).   
  - Make an issue, branch, and PR to a link to the deployed app and a link to the Heroku dashboard into the README.md for the repo. (The heroku app may not initially run because of OAuth configuration, but that's ok; getting that setup is a separate issue.)
  - When merged, this will be worth 5 points for this team.
  - Add all of the staff to the production deployment: `alu@ucsb.edu`, `kheffernan@ucsb.edu`, `bzamoraflores@ucsb.edu`, `andrewpeng@ucsb.edu`, `phtcon@ucsb.edu`.
  - For Courses Search only, configure the `UCSB_API_KEY`, `MONGODB_URI`, and other applications specific values; see the
    app specific setup task lists below in the drop down boxes (click the triangles to reveal.)
  - Add all of the staff to the list of admins on the production deployment.
  - When merged, this is worth 5 points for the team.
* Someone on the -1 or -3 team should set up the Codecov badge on the `main` branch 
  - Create an issue, branch, and PR for doing this, and adding the codecov badge to the README.md
  - When merged, this is worth 5 points for the team.
* Someone on the -2 or -4 team should set up OAuth credentials that work on <http://localhost:8080> as well 
  as on your Heroku production deployment (see link above), and all of the QA deployments for *both* the 1 and 2 teams, or the 3 and 4 teams, depending on which app you are on.
  - Distribute the credentials to your team and the other team in your group, but *do not* post in your team's slack channel; instead, use a group DM to all of your team, plus one person on your partner team; they should then DM it out to the rest of the folks on their team.
  - There's nothing to merge for this, but still create an issue for it.
  - All points get attached to a PR, so we'll attach these point to the PR for the production deployment of the repo.
* Someone on *every* team should make a QA Heroku Deployment for your team with a name matching this pattern: `s22-4pm-1-courses-qa` or `s22-5pm-4-happycows-qa` (you can infer what your team's name should be from the examples.)
  - Make an issue, branch, and PR to a link to the deployed QA app and a link to the QA Heroku dashboard into the README.md for the repo. (The heroku app may not initially run because of OAuth configuration, but that's ok; getting that setup is a separate issue.)
  - When merged, this will be worth 5 points for this team.


<details>
<summary>
Course Search Specific Tasks
</summary>
  
For Courses Search, the `.env` file also needs a value for the URL of a MongoDB database.
  
Here's what the values look like when configured in Heroku:

![courses-search-env-values](https://user-images.githubusercontent.com/1119017/170117172-446c4269-e8d9-4151-bb52-b1ca0938c7ec.jpg)

The values for `UCSB_API_KEY` and `MONGODB_URL` were distributed on Slack; one person on your team received them from Prof. Conrad via Slack DM, and can share them with the rest of the team via Slack DM (please don't put them on the open channel.)

</details>


<details>
<summary>
Happy Cows Specfic Tasks
</summary>
  
For Happy Cows, there are currently no known project specific set up tasks, but if any arise, we'll post them here.
  
</details>

