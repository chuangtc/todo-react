# How to run todo-app and deploy to Firebase
Date:　2022-09-10
## Git repsository
```
git clone https://github.com/chuangtc/todo-react.git
```
## Software version
* React 18.2.0

## Step1
```
npm install
```
## Step2
```
npm start
```
## Step3
Runs the app in the development mode.

Open http://localhost:3000 to view it in the browser.

### Set up firebase
```
npm install -g firebase-tools
firebase login
npm run build
```

## Step 4: Initialize Firebase in Your React App
```
firebase init
```
* For the first question select option Hosting: Configure and deploy Firebase Hosting sites.

* In the second question that is Project setup, Select Use an existing project, and in that select Firebase project name that you have created.

* And the last part is the Hosting setup part here you will need to specify the folder where Firebase will look for assets to deploy. By default, the build folder will contain the production assets. So Enter build as an answer to this option.

* For Configure as a single-page app question enter y for this option.

* The last question is whether or not to overwrite your existing build/index.htmlfile. So You'll want to enter N (No) for this option because we want actual index.html file that Reacts is generated while creating the build.

Run simulator in local machine
```
firebase simulators:start
```
Open browser, and type in the following

http://localhost:5000

## Step5 Deploy to firebase
```
firebasae deploy
```
## Check deployed website
https://react-todo-656ce.web.app/

## Or visit the website for demo
https://chuangtc.com/react-todo/