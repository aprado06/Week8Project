# Week8Project Project 8 - Pentesting Live Targets

Time spent: **6** hours spent in total

> Objective: Identify vulnerabilities in three different versions of the Globitek website: blue, green, and red.

The six possible exploits are:
* Username Enumeration
* Insecure Direct Object Reference (IDOR)
* SQL Injection (SQLi)
* Cross-Site Scripting (XSS)
* Cross-Site Request Forgery (CSRF)
* Session Hijacking/Fixation

Each version of the site has been given two of the six vulnerabilities. (In other words, all six of the exploits should be assignable to one of the sites.)

## Blue

Vulnerability #1: SQL Injection<br/>
Can inject sql in the id parameter to make the website sleep/ have a delay.

<img src="gifs/BlueSleepSQLi.gif" width="800">

Vulnerability #2: Session Hijacking/ Fixation<br/>
Use the hacktool to change the PHPSESSID of someone that is logged in already so that the session will now be logged in.

<img src="gifs/BlueSessionId.gif" width="800">

## Green

Vulnerability #1: Cross-Site Scripting<br/>
Inject code in the feedback that will be executed when someone goes to view the feedback

<img src="gifs/GreenFeedScript.gif" width="800">

Vulnerability #2: Username Enumeration<br/>
On the log in if the username exist and the log in is unsucessful the message will be bolded while if the username does not exist the message will not be bolded.

<img src="gifs/GreenUserEnumeration.gif" width="800">


## Red

Vulnerability #1: Insecure Direct Object Reference<br/>
Can change the id parameter to show people in the system that are not supposed to be shown.

<img src="gifs/REDIDOR.gif" width="800">

Vulnerability #2: Cross-Site Request Forgery<br/>
Create an html form that changes the person with the id=4 so when a logged in person goes to the malicious site the info will be changed while the website  shows nothing. 

<img src="gifs/RedCrossSite.gif" width="800">


## Notes

None
