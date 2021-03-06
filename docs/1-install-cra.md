[back to index](/README.md) | [next](/docs/2.md)

# Step One - Create the React Project

You're going to use Create React App to bootstrap your React application. To do this, you’ll need a relatively recent version of Node.js. The most recent version as of this writing is 14.x.

Node will automatically install NPM - the Node Package Manager. You can then use NPM to install all of the other libraries talked about below.

With Node and NPM installed, navigate via the command line to the directory within which you want to put the project. Next, run the following commands in sequence:

```
 npx create-react-app first-mern
 cd first-mern
 code .
```

The first command installs all of the directories and files you need for the moment. **The installation will take a while** and you’ll see lots of information printed to your screen. Don’t worry about any warnings. The second command changes the working directory to the newly created first-mern directory. The final command tells your system to open the current directory in VS Code. You can substitute another code editor if you like.

From within your code editor, the file structure should look like this:

```
 node_modules/
 public/
 src/
 .gitignore
 package.json
 package-lock.json
 README.md
```

The directories you’ll work with most are the top level and the src directory. Get familiar with the structure and files. And don’t worry if you feel a bit lost at the moment. Things will become clearer.

Next, from the command line, run:

```
 npm start
```

This will start a development server that will serve your React application. Open your browser and in the address bar, type in localhost:3000. The site should load and show a spinning icon.

NOTE: The NPM start script can be found in package.json. You can create other scripts in the same place. Other scripts will require a slightly different syntax to start. Use `npm run myScript`.

These are the scripts that come with the Create React App installation.

```js
"scripts": {
   "start": "react-scripts start",
   "build": "react-scripts build",
   "test": "react-scripts test",
   "eject": "react-scripts eject",
 },
```

If you'd like to learn more about those scripts, we suggest reading the README.md file in your project's root directory.
