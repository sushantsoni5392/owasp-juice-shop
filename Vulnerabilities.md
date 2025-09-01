This document lists the vulnerabilities found in the OWASP Juice Shop application

## Finding the scoreboard page
When you open the application in the browser using `http://localhost:3000` and go through the source code, specifically `main.js` to look for different routes available. Searching for `score` reveals the path `score-board`.

Opening the url `http://localhost:3000/#/score-board` opens the scoreboard and you can see that challenge is solved.

This vulnerability can be attributed to the top OWASP Top 10 Vulnerability - [Broken Access Control](https://owasp.org/Top10/A01_2021-Broken_Access_Control/). Public access should be denied by default for a page that is not meant to be public.

## XSS

XSS in the search functionality is another popular vulnerability that exists in web applications.
In the OWASP Juice Shop app, using the search bar, one can use the payload `"><img src=x onerror=alert(1)>` to demonstrate this vulnerability.

**Note** - The payload just demonstrates the vulnerablity exists. The actual exploit of an XSS vulnerability would depend on the application.



