My answer:

I would start by 

1.
 Check with the 1st Line Support Desk or with the client if the problem is happening solely on our application and then if solely on the private areas of our application (that demand authentification).
 If such a response is not available I would assume that the answer is yes.

2.
 If this is a recurring problem I would check the past solve within the team.

* A first guess would be that the problem is caused by a change on the authentication configuration code, taking a hint from the fact that the signin page is not accessible.
  Given the fact that this problem passed unnoticed through the testing phase and the pre production phase, a check for a misuse of some environment variable should also be taken into consideration.

3.
 If this is a never seen before problem then I will check for the latest changes made to the production stage (with the devops team) and the latest changes/deployments made to our application.
 At this moment it is a reasonable expectation that the problem was caused either by a code change or by a production environment change;
 I would expect this to be the last step of the investigation, most of the times.

4.
 If changes/updates were made to the production environment then I would ask for help from the devops team on checking the logs/settings of IIS and the SQL Traces.

5.
  If no changes/updates were made to the production environment then I would start checking the event viewer.
