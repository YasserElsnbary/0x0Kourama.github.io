---
title: ASCWG-Web-G(old)
published: true
---

![](https://i.ibb.co/jLj2Jhc/110313248-2542820449361412-4064549934332186149-n.jpg)

## [](#header-4)Challange Desciption:
*   Difficulty: Easy
*   Points: 300 point
*   Category: Web
*   Challange Link: 10.0.0.5 on LAN Network it  is not Available Online
*   vulnerability : [SSI](https://owasp.org/www-community/attacks/Server-Side_Includes_(SSI)_Injection)

## [](#header-3)Steps:

*   Go to 10.0.0.5
*   you will get this login Form 
*   After making some routing search on this page like: show source Code, Request, resopsne and Cookies i didn't find any thing can catche my attention.
*   so,first thing I tried deafault credentials like admin:admin
*   ![](https://i.ibb.co/DCZdBFd/login.png)
*   you will get welcome message with the value of $_POST['name']
*   ![](https://i.ibb.co/dmTx1mQ/login-admin.png)
*   i didn't gey Anything useful
*   <span style="color:#ce1127">Notice<span> ```red rectangle``` around file Name and extension ```.shmtl ```
*   return to Login Form 
*   try Login using anything you will login i will try login with yasser:yasser or xss payload will work but not return with flag or any thing
*   ![](https://i.ibb.co/52PGz0M/another-User.png)
*   you will notice that file name was change again
*   and still with shtml extension
*   i will search about shtml
*   ![](https://i.ibb.co/yyh997T/search-shtml.png)
*   open first [link](https://www.computerhope.com/jargon/s/shtml.htm) and read it
*   ![](https://i.ibb.co/kxWqzSh/follow-search.png)
*   so it may be [SSI](https://owasp.org/www-community/attacks/Server-Side_Includes_(SSI)_Injection) ``` Server Side Injection ```
*   you can using any scanner like burp scanner To be sure
*   So i will seearch about [SSI payloads](http://marduc812.com/2018/03/24/list-of-ssi-payloads/)
*   Fire Burp Suite and injecti payload , What Happend? 
*   


