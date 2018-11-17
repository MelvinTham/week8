# Project 8 - Pentesting Live Targets

Time spent: **X** hours spent in total

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

Vulnerability #1: Session Hijacking/Fixation

    GIF: ![](blue1.gif)
  - Details
    * Open two browsers (Chrome and Firefox in this case).
    * Login to green and go to https://104.198.208.81/green/public/hacktools/change_session_id.php and copy the PHPSESSIONID.
    * Copy and paste that in to Blue https://104.198.208.81/blue/public/hacktools/change_session_id.php and press "Change".
    * Change the url to https://104.198.208.81/blue/public/index.php and you will be logged in without even logging in!

Vulnerability #2: SQL Injection
  GIF: ![](blue2.gif)
  - Details
    * Direct to the "Find a Sales Person Tab"
    * Click on a sales person and add this ' OR SLEEP(5)=0--' to the url at the end. 


## Green

Vulnerability #1: __________________

Vulnerability #2: __________________


## Red

Vulnerability #1: __________________

Vulnerability #2: __________________
