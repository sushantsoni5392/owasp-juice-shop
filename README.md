# OWASP Juice Shop

```
This is test repository to run DAST against the vulnerable web-application OWASP Juice Shop
```

OWASP Juice Shop is an intentionally built vulnerable web-application. Security researchers or anyone can use it to learn about different vulnerabilities.

# Running OWASP Juice Shop

```
docker run -d --rm -p 3000:3000 --name juice-shop bkimminich/juice-shop
```

This will run the application locally on port 3000. You can access it using `http://localhost:3000`

# Scoreboard
The application offers a scoreboard that lists the vulnerabilities existing in the application. Finding the scoreboard itself is on of the challenges.
