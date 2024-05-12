# Postmortem 
## Website is downloading file instead of opening website in plesk panel
A postmortem (or post-mortem) is a process intended to help you learn from past incidents. It typically involves an analysis or discussion soon after an event has taken place.

Postmortems typically involve blame-free analysis and discussion soon after an incident or event has taken place. An artifact is produced that includes a detailed description of exactly what went wrong in order to cause the incident, along with a list of steps to take in order to prevent a similar incident from occurring again in the future. An analysis of how your incident response process itself worked during the incident should also be included in the discussion. The value of postmortems comes from helping institutionalize a culture of continuous improvement. This way, teams are better prepared when another incident inevitably occurs with mission- or business-critical systems.


## Requirements:
### Issue Summary
- Duration of outage: 8days
- In my case, This file contains a brief description of an outage occurred on April 12/2024 till April 20/2024, it was given to me website is downloading file instead of opening website in plesk  panel while I was uploading, I tracked and found the main causes and finally restore the failing services.
- While I have uploaded PHP files to my webserver with Plesk panel, I found that when I visit the page in my browser, that the browser attempts to download the file instead of processing it and displaying it. I was tried for many times to fix it. The campany called Canny Bussiness and consultancy PLC affected by this issue for more than one week. 

### Timeline
- before april 12 for the previous 15 days I tried to develop the website for the specified comapny called Canny bussiness Consultancy PLC
- April 12/2024 at 9:00 AM, I already buy the server and domain name from the Ethiopian Tele Comunication Center.
- April 12/2024 at 4:00 AM, I tried to configure or upload the file to the Plesk pannel.
- Starting from April 12/2024 at 4:00 AM up to April 18/2024 finding the cause in order to detected the issue 
- April 18/2024 The service failure was detected
- Aprile 19/2024 The Root cause was found
- Aprile 20/2024 The Root causes was fixed
### Root Cause
The root case for this outage ic that, PHP support is disabled for the example.com domain in Domains > example.com > PHP Settings.
The result for this cause is that PHP is not being handled correctly. Trying to access a PHP page on a website, it asks to download it, instead of executing it.
### Resolution and recovery
The main cause of the outage specified in the previous section. Inprder to resolve this problem I tried to review different materials for one week. after that I found the root cause and was tried to resolve that. 
we do have two methods to resolve the problem. these are 1) Via Plesk Graphic Interface  2) Via Commandline Interface (CLI)
I am selecting the first option and look at the following procedure. The procedure for resolving it is as follows.
 1. Login to Plesk Panel
 2. Navigate to Domain>example.com>PHP Setting
 3. Select PHP Support checkbox and press the Ok button
 4. please see the next image
![image](https://github.com/Temesgenswe/alx-system_engineering-devops/assets/101357503/af72c92d-5a2a-422d-9db2-7554f555d46d)

### Corrective and Preventative Measures
To prevent similar incidents in the future, the following measures will be taken:
- Bieng understand the feature of the server before uploading the file.
- Asking the procedure to be follow to upload the website (PHP) files in the Plesk Panel
- Improved monitoring and alerting system to quickly detect and respond to anomalies in PHP file and database connection usage.
- Conduct training sessions to educate development teams on connection pool management best practices.

Specific tasks to address the issue include:
- Conduct a comprehensive code review of the web application code.
- Implement additional automated tests to detect memory leaks.
- Update monitoring tools to include more granular resource usage data.
- Provide additional training for operations team members on troubleshooting web application issues.

