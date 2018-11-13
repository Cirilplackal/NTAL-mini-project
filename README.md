# Network Threats mini project -Cross sit scripting

Cross-Site Scripting (XSS) attacks are a type of injection, in which malicious scripts are injected into otherwise benign and trusted websites. XSS attacks occur when an attacker uses a web application to send malicious code, generally in the form of a browser side script, to a different end user. Flaws that allow these attacks to succeed are quite widespread and occur anywhere a web application uses input from a user within the output it generates without validating or encoding it.

An attacker can use XSS to send a malicious script to an unsuspecting user. The end user’s browser has no way to know that the script should not be trusted, and will execute the script. Because it thinks the script came from a trusted source, the malicious script can access any cookies, session tokens, or other sensitive information retained by the browser and used with that site. These scripts can even rewrite the content of the HTML page.


## Requirements:
* Node.js
* Git

## Getting Started

If you have not already done so, make sure you have all the [requirements](#requirements) from above.

For Windows users, open Git Bash. You will use this program to run all the "terminal" commands you see in the rest of this guide.

For Linux and Mac users, open Terminal.

```bash
cd xss
```

Install the project's dependencies using npm:
```bash
npm install
```

Now we can run the local web server using Node.js:
```bash
node server.js
```
If successful, you should see the following message: `Server listening at localhost:3000`. This means that a local web server is now running and is listening for requests at [localhost:3000](http://localhost:3000/). Open your browser and click the link.

You should see a simple search form. Enter some text then press enter (or click the "search" button). Notice how the search query you entered is shown in the page. This form might be vulnerable to an XSS attack. 
