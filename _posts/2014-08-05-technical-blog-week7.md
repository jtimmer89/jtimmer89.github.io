---
layout: post
title: "Technical Blog: SQL Injection"
quote: What is SQL injection and how do you avoid it?
image: /media/technical-blogs/AutumnLake_14.jpg
video: false
---

#What is it?

Many websites that have users or large amounts of data will use a database to store that information, access it, edit it, and anything else you might want to do with your data. I have learned pretty quickly in programming with Ruby that storing data can quickly become confusing and unmanageable. A programming language like Ruby is great for accomplishing actions, but it is not great for storing data though it is possible. I look forward to learning more about how to use databases effectively.

Data is really important, and you wouldn’t want anybody to be able to access your data and delete it. As an IT person for a sales company, I have spent many hours modifying data when moving from one CRM to another. The loss or modification of data can be a massive problem. When creating software for the web, you want to make sure it is as secure as possible. Spending the time to understand potential threats and how to protect against them is important because of how much time it will save you down the road.

SQL injection is a very popular method of hacking data, modifying it, erasing it, and anything else you might want to do to/with somebody’s data. It is popular because of how simple it is. Without getting too technical, SQL injection happens through the front end of a website. You get on your favorite browser, go to your favorite website, and login. When you login, data is being accessed to check if you type in the right password and that your username exists. At this juncture, it is possible to send SQL commands to the database and then get access to users and their passwords or whatever might happen to be in the database. I picture a military code that allows an officer to send orders. Once being able to access the soldiers in the field, with the right code, you could send messages and commands to have them do whatever you wanted to the dismay of the true commander. At its least disruptive, you spend time cleaning your database and removing the threat for the future. At its worst, your users information is stolen and potentially used for fraud and other illegal activities.

##What can you do about it?

There are companies that could help you with this problem. However, if you are working as a newb programmer, you probably don’t want to recommend help from elsewhere. You are now the expert so what do you recommend doing about this problem? I don’t know enough about the specifics yet to give you a step by step guide, but I can point you in the right direction on how to protect against SQL injection attacks. One key is sanitizing your data. When a username or password is entered into the web page, the data should be taken and examined. Phone numbers should only have numbers. You can make sure through sanitization that data is being entered properly. That way, if a hacker was trying to inject SQL commands, they would be modified before accessing the database.

You could also create user statuses like admin or average joe. The average joe could only query a database limited to the necessary information for average joe. This would disallow someone accessing the entire database through average joe. It seems though that there are ways for hackers to get around these two options. The best option is to not construct SQL queries with user input. Great, what does that mean? The basic idea involves the fact that when your information is sent to the database to be processed, you have the option to include the literal data in an SQL statement or to use bind variables. Using bind variables allows you to reroute the hacker’s attempted attack and make it unable to query the server and access data. I look forward to understanding how to do these things in actuality and create secure databases!