---
layout: post
title:  "Meltdown! a JavaScript learning game!"
date:   2015-11-17 21:17:00
categories: jekyll update
---

Recently I worked on an exciting project with a small team. Our task was to conceptualize and build an application that we felt strongly about. After a few days of discussion, we settled on some key components we wanted to work with. Education, coding, and gaming. Given these concepts, we came up with Meltdown! ~ a JavaScript learning game. It needed to be fun, engaging, challenging, and communication based. 

**THE GAME:**
Coding is a team sport so we wanted our game to be too! Meltdown can be played as a single player as well but it is much more fun when you play with others. You can play with up to 3 other people and if you do, you must share code snippets with each other in order to pass through the levels and survive as a team. The game takes place at a nuclear reactor that is breaking down. You have a limited amount of time and mistakes for each level. Once you and your friends join the game, you will each find yourselves in a room with a red console that you need to access. Once you access it, a code challenge pops up. Meanwhile, to the left of the game room is a ‘reactor manual’ that has all of the JavaScript functions that you and your team need to understand and solve based on the code challenge data in order to turn the console green. 

But there’s a catch! The manual has been corrupted and there are missing pieces. Your team members’ manuals will have the missing lines of code and you must communicate with them to determine which functions you are solving and what lines you need. Once you have all worked together and solved all of the problems, you can all walk into the next room where there will be a new set of problems and new manual pages to use in order to continue saving the reactor from overheating and explosion. 

**THE CODE:** 
Engineering Meltdown! was an amazing experience. Each member of the team brought excellent skills and incredible enthusiasm. Since none of us had previous game experience we had to discuss possible game engines before we could even begin. Phaser.io stood out as a versatile game engine. The next piece was a database and synching platform. We opted to try out Firebase as it could handle both needs simultaneously. Using AngularJS in combination with these components was the obvious choice for our client side needs. Firebase offers a JavaScript library that integrates with AngularJS ~ AngularFire. 

AngularFire proved to be an effective tool for communication with its three-way data binding. As we know, AngularJS has two-way data binding and AngularFire adds a third layer of binding to the database, meaning that changes are updated immediately to the database and disseminated to all client instances. This was very useful for our timer, strike, and game start/end needs. 

For our server we opted to use NodeJS/ExpressJS. Using Firebase on the server made it so we could upload randomly generated puzzles to the database which broadcast them to the clients. Finally we decided to deploy on Heroku which made getting our game online a quick endeavor. 

All in all, Meltdown! has all of the components needed to play a fun game while sharpening JavaScript skills! The great thing about Meltdown! is that you don’t have to be in the same room as the people you are playing with. Hop on a google hangout or another conference call system and you can play with people across the world! 


**THE FUTURE:**
Some future hopes for the game include integrating WebRTC in order to have in-game video conference capabilities, adding more levels and more types of problems, and creating strike challenges that involve typist or speed mini-games that allow you to work off a strike.
In the truest spirit of community and multiplayer, we have kept the code open source and you can find it on [gitHub here][githubMelt] ~ feel free to create new features and send in a pull request!

[Play Meltdown!][meltdown] now for a fun coding adventure! 


[githubMelt]: https://github.com/team-jems/Meltdown 
[meltdown]: http://melt-down.herokuapp.com/
