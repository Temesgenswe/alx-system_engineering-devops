# Postmortem 
## Website is downloading file instead of opening website in plesk panel
A postmortem (or post-mortem) is a process intended to help you learn from past incidents. It typically involves an analysis or discussion soon after an event has taken place.

Postmortems typically involve blame-free analysis and discussion soon after an incident or event has taken place. An artifact is produced that includes a detailed description of exactly what went wrong in order to cause the incident, along with a list of steps to take in order to prevent a similar incident from occurring again in the future. An analysis of how your incident response process itself worked during the incident should also be included in the discussion. The value of postmortems comes from helping institutionalize a culture of continuous improvement. This way, teams are better prepared when another incident inevitably occurs with mission- or business-critical systems.


## Requirements:
### Issue Summary
- In my case, This file contains a brief description of an outage occurred on April 12/2024 till April 20/2024, it was given to me website is downloading file instead of opening website in plesk  panel while I was uploading, I tracked and found the main causes and finally restore the failing services.
- While I have uploaded PHP files to my webserver with Plesk panel, I found that when I visit the page in my browser, that the browser attempts to download the file instead of processing it and displaying it. I was tried for many times to fix it. The campany called Canny Bussiness and consultancy PLC affected by this issue for more than one week. 
- The root case for this failerity is that PHP is not being handled correctly. Trying to access a PHP page on a website, it asks to download it, instead of executing it.

### Timeline

### Root Cause

### Resolution and recovery

### Corrective and Preventative Measures
[This is  Important]
