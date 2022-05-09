---
num: "Lecture 18"
lecture_date: 2022-05-10
desc: "Tue Lecture: For HappyCows (teams 3,4)"
ready: false
---

These instructions are for teams ending in 3 and 4, which will be working 



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


