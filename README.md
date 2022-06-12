# Deploy a simple html page on repl.it

This repo is intended to teach web dev early learners how to easily deploy their web apps on repl.it while giving them some experience on using the `npm` to manage the build and deploy.

## First: what is repl.it?

repl.it is a free hosting service which can make our web app available to the public through a public domain accessible from any web browser in the world.

## What's npm?

The node package manager helps us add important "packages" to our application so that we can create a server. In this example, we will be using `express` to serve our app.

## Server? Package? Express? 

The server is basically a javascript program which we will write in order to allow our `index.html` to be accessible through the browser.

Packages are programs (codes) written by other people with the goal of saving us some work. Packages provide us with functions that perform tasks which are either too difficult or too repetitive for us to code. In this case, `express` will be responsible for creating a server where our application will run.

### Starting from scratch

1. Create a sample html in `index.html`, it can be just a 'hello, world' or another app you'd like to deploy.
2. We need `npm` to complete this job, so you'll need to have it installed in your system.
3. Once we have `npm` installed and our `index.html` file ready, move to the folder where you want to keep your app and run `npm init` - in Linux.
4. After that, we need to install express. Run `npm i express --save` in the same terminal.
5. Our project folder now must have 2 new files: `package.json` and `package-lock.json` - they're the files that keep track of what packages we add to our project.
6. Open `package.json` and find the `scripts` key. By now, there must be only the `test` key inside.
7. Add a script to `scripts` after `test` called `start`, the value should be `node server.js` - we'll create the server next.

### The server

1. Create a file in your project's folder called server.js.
2. Import the express package: `const express = require('express');`.
3. Create an app to hold the server: `const app = express();`.

