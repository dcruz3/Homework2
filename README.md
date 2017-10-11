# Homework2

Please complete the following tasks for Homework #2:
1.          Installing Node
We already have done this in class. If you have not done it yet, please complete installing Node
You can verify if Node is installed or not by typing the following in your terminal: node –v
Make sure you have Node (http://nodejs.org) and npm (Node's package manager) installed
Npm comes bundled with Node so as long as you install Node, you'll have access to npm
If you have trouble with the installation process, try restarting your computer and making sure that Node is in your PATH. Check the Node installation page
(https://github.com/joyent/node/wiki/installation#installing-on-windows) and npm install page (https://github.com/npm/npm/wiki/Troubleshooting) for more troubleshooting. Now that we have Node and npm installed, let's get to our first app!
 
2.          Initialize a Node App
Let's create a sample project and test out the npm init command
1. Create a folder: mkdir awesome-test
2. Jump into that folder: cd awesome-test
3. Start our Node project: npm init
o   It will give you a few options that you can leave as default, blank, or customize as you wish. For now, you can leave everything default except for the main (entry point) file. Ours will be called server.js
o   You can see that our new package.json file is built and we have our first Node project!
o   The package.json file is how we will start every application. It can be hard to remember exactly what goes into a package.json file, so npm has created an easy to remember command that let's you build out your package.json file quickly and easily. That command is npm init
o   Node applications are configured within a file called package.json. You will need a package.json file for each project you create. This file is where you configure the name of your project, versions, repository, author, and the all important dependencies.
o   Since we have a package.json file now, we can go into our command line and type node server.js to start up this Node app! It will just throw an error since we haven't created the server.js file that we want to use to begin our Node application.
o   Now we will need to create the server.js file. The only thing we will do here is console.log out some information.
o   console.log() is the way we dump information to our console. We're going to use it to send a message when we start up our Node app.
o   Create server.js file and put the following content into it: console.log(‘This is our tiny Node app in ISOM 215!');
 
3.         Start up Node application
o   Now we can start up our Node application by going into our command line and typing: node server.js
o   We should see our message logged to the console. Remember that since Node is JavaScript on the server, the console will be on our server.
 
4.         Restarting a Node Application on File Changes
o   By default, the node server.js command will start up our application, but it won't restart when file changes are made. This can become tedious when we are developing since we will have to shut down and restart every time we make a change.
o   Luckily there is an npm package that will watch for file changes and restart our server when changes are detected. This package is called nodemon (https://github.com/remy/nodemon) and to install it, just go into your command line and type: npm install -g nodemon
o   The -g modifier means that this package will be installed globally for your system. Now, instead of using node server.js , we are able to use: nodemon server.js
o   Go into your server.js file and make changes. Then watch the cool change happen when application restarts itself!
 
5.          Check-in your project to Github and upload your project link to Blackboard.
