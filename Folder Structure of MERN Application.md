[[MERN]]

# Folder Structure of MERN Application 
#resource 
The most basic structure would be to have a `root` folder that contains `frontend` and `backend` folders. Since you're talking about the **_MERN_** stack, you would have a `package.json` inside of your **`NodeJS`** backend environment and a `package.json` for your **`React`** side of things. Backend server and the frontend client are two totally separate things, so yes, they both have their own node_modules folders. On the backend, you'll probably have installed something like `Express` for your Node runtime, `Mongoose` for a more convenient way to talk to your `MongoDB`, etc, and on your frontend, you'll have your `React` as your frontend framework, `Redux` for state management, etc. Additionally, depending on what you have already listed inside of your package.json files, when you run `npm install` **separately** it will be installed in those two folders. If you want to install additional packages, just run `npm install + "the name of the package"` (without the '+' and without the quotes) inside of that particular folder where you need it (backend or/ and frontend).

I hope this was helpful. Check out the pics, especially the 2nd one.

**App structure**  
[![enter image description here](https://i.stack.imgur.com/fYFze.png)](https://i.stack.imgur.com/fYFze.png)

**Folder structure**

[![enter image description here](https://i.stack.imgur.com/8ogDx.jpg)](https://i.stack.imgur.com/8ogDx.jpg)

**UPDATE:**

In development, I suggest installing two additional things:

1. _`npm i -D nodemon`_
2. _`npm i -D concurrently`_

Note: The `-D` flag will install them as _`devDependencies`_.

**`nodemon`** is going to track every file change and restart the backend server for you. So, it's obvious that it should be installed inside of the "backend" folder. All you have to do is go inside of the `package.json` file (backend) and add a new script. Something like this:

```javascript
"scripts": {
"start": "node app.js",  // in production
"dev": "nodemon app.js", // in development
}
```

---

**`concurrently`** allows you to start both your frontend and backend at the same time. I suggest initializing a new Node project inside of the top-level **root** folder -[folder which contains both, your frontend and backend]. You would do that with the `npm init` command, and after that, install the `concurrently` package there.

Now, go open your newly created `package.json` file inside of your **_root_** folder and edit the start section, like this:

```javascript
   "scripts": {
       "dev": "concurrently \"cd backend && npm run dev\" \"cd frontend && npm start\" "
   }
```

What this will do is go inside of the **backend** folder and run the `dev` command (_the same one we just configured_), so that will start `nodemon`. Additionally, it will also go inside of the **frontend** folder and run the default `start` command -which is exactly what we want.

If you kept the folder structure, installed all the dependencies (including the additional two I mentioned above), changed the `package.json` file inside of your **`root`** folder, you'll be able to start them both with a simple command:

**`npm run dev`** // make sure you're inside of the root folder when doing so :)
[Reference](https://stackoverflow.com/a/51128385)