# Building Your First MERN App
By [Julian Johannesen](https://github.com/julianjohannesen) and [Ben Davis](https://twitter.com/bengineerdavis) 

### Index

* **[Goal](#Goal)**
* **[Background](#Background)**
* **[Links](#Links)**
* **[Overview](#Overview)**
    * [Step 1 Create the React Project](/docs/1.md) 
    * [Step 2 Set Up Express Server](/docs/2.md)
    * [Step 3 Install MongoDB](/docs/3.md)
    * [Step 4 Connect to MongoDB](/docs/4.md)
    * [Step 5 Add Routes in React](/docs/5.md)
    * [Step 6 Add Routes in Express](/docs/6.md)
    * [Step 7 Request Data](/docs/7.md)

## Goal

**Create a simple web app using the MERN stack and explore basic authentication.**

In this tutorial you'll become familiar with how to build web applications that depend on APIs to provide them with services like user authentication and authorization. You’ll be building a very simple website that will allow a user to register an account, log in, and log out securely. The stack you’ll be using is the popular MERN stack, which comprises MongoDB, Express.js, React.js, and Node.js. You’ll be using several other technologies along the way, but those four are the biggies.

This tutorial is not intended to teach you everything you need to know to deploy an application. Our intention is to cover only what you need to know in order to build a working application.

## Background

This is a tutorial for beginners, so don’t worry if you don’t have very much familiarity with one or more of the technologies we just mentioned. We’ve created a [list of resources](links-to-resources.md) that should help get you up to speed.

There are a few concepts that you should make sure you have at least some understanding of, in order to get the most out of the this tutorial. 

The first of those concepts is the basic structure of the web. Make sure that you know what the client-server model is, what HTTP is, how clients send HTTP requests to servers, how servers respond with HTTP responses. Do you know what an HTTP verb is? Do you know the difference between a message header and a message body? If you have a rough idea about what each of these terms means, you're in good shape. If not, refer to the [list of resources](links-to-resources.md).

It's particularly important that you understand how server software uses routing to receive various types of HTML requests and deal with them appropriately. An example is sending an HTML document back to the requesting client software.

Another important concept is that of a RESTful API. If that sounds unfamiliar, go check out the [list of resources](links-to-resources.md).

## Overview

1. You’ll begin by setting up the React project and ensuring that you’re able to use a development server to serve some React boilerplate to the browser.
2. Next, you’ll set up a very simple Express server and ensure that you can use it to serve a simple page to the browser.
3. Then you’ll install MongoDB, and make sure that you're able to start it, and interact with it via the Mongo shell.
4. Using Express and MongoDB together is much easier with an ORM, so you’ll install Mongoose. After making some edits to the Express server script, you’ll ensure that the Express server can connect to MongoDB.
5. At this point, you’ll jump back to the front-end and use React Router to set up some client-side routing. You’ll also create a couple of simple React components for the routes to render.
6. Returning to the Express server you’ll create a couple of routes that the front-end will eventually use to fetch data.
7. asdf

## During Development

Unless you plan to complete the tutorial in one sitting, there are a few things that you'll need to remember to do when you come back to this project after being away. Failing to take the following steps will cause errors that will annoy you to know end:

1. `Start the React dev server (served on port 3000) and test the navigation links to make sure they're both working.`
2. `Start Mongo, if it isn't already running (default port). If you don't start Mongo before starting the Express server, you'll get an error.`
3. `Start the Express server (served on port 8080)`
4. `Use curl (or Postman) to send a POST request to Express to make sure it's working`
5. `Inspect the database with the mongo CLI and query a record to make sure everything is working as it should`


NOTES -

- Talk about the difference between a site and service. The React app is a site that's served from a server, but requires no interaction with the server that's hosting it. The Express server is not a "site", although Express can certainly serve HTML pages. In this tutorial, the Express server is serving an API. The API is a service. Client apps can send data to the API and request data from the API.