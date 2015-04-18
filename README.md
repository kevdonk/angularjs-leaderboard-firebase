Angularjs-Leaderboard-Firebase
==============================

Welcome to a realtime leaderboard built with [AngularJS](https://angularjs.org/) and [Firebase](https://www.firebase.com/)! This app is simple to set up so let's get started.

Prerequisites
-------------
- [Git](http://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
- [Node.js and NPM](https://nodejs.org/)
- Serve NPM package (`npm install -g serve`)

Getting Started
---------------
First, make sure you have Git and Node.js installed (see "Prerequisites"). Then open your terminal/command prompt and run the following commands:
```
git clone git@github.com:simpulton/angularjs-leaderboard-firebase.git
cd angularjs-leaderboard-firebase
```
Now open up the code in your favorite text editor.

Setting up Firebase
-------------------
To run the app, you will need to set up an account with Firebase. Don't worry, it's free AND easy!

#### Get a Firebase Account
First, navigate to https://www.firebase.com/. Then you can do one of two things: you can sign up for an account with your email or, if you have a Github account, you can log in with those credentials.

#### Create an App
After you have logged in/signed  up, you will be taken to your dashboard. Go ahead and create a new app (call it whatever you want). After you click `CREATE NEW APP`, your app will appear in your dashboard.

#### Get your Firebase URL
Click `Manage App` on your newly minted Firebase app. Once you have transitioned to the new page, copy the URL from the address bar. It should look like `https://<your-app-name>.firebaseio.com/`.

#### Put the URL in the app
Now open up your code editor, navigate to `js/leader-board.js`, and replace the `FIREBASE_URI` constant ([line 3](https://github.com/simpulton/angularjs-leaderboard-firebase/blob/master/js/leader-board.js#L3) as of this writing) with your Firebase URL. Firebase is now ready to go!

Running the App
---------------
Now go back to your terminal, make sure you are in the `angularjs-leaderboard-firebase` directory, and then run `serve`. In your browser, navigate to `http://localhost:3000`. Boom! The app is now running. Read on for a tour of the app.

Tour de App
-----------
Let's take a quick look at what the app does.

#### The Index View
The index page is where we show all of our data.
<img alt="index" src="https://cloud.githubusercontent.com/assets/9245381/7214613/ec605452-e568-11e4-8a4e-13a1ede75f8a.png" style="width: 750px; height: 360px;">
#### The Admin View
The admin page is where we can CRUD (Create Read Update Delete) our data.
<img alt="admin" src="https://cloud.githubusercontent.com/assets/9245381/7214615/f8211fc4-e568-11e4-82d6-9cdbdf15d4ed.png" style="width: 750px; height: 481px;">
#### The Remote View
The remote page is where the realtime component becomes important. Here, we can choose a contestant and then update their score. [Click here](http://www.screencast.com/t/NsodHlrFFRd) to see a realtime demo.
<img alt="remote" src="https://cloud.githubusercontent.com/assets/9245381/7214617/fc982fac-e568-11e4-9a29-b31a4fa0a46f.png" style="width: 750px; height: 369px;">

