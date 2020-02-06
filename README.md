# React to To Do List + deployment on Github pages

## Features
* add new items to your list
* mark as done
* delete items from your to do list list

## Dependencies:
*    axios
*    react-router-dom
*    uuid
*    gh-pages


## Deploy commands:

* npm init react-app my-app
* cd my-app -> npm install gh-pages --save-dev
* In package.json change:
  - "homepage": "http://YOURGITHUB.github.io/my-app"
  - "scripts": {
        //...
        "predeploy": "npm run build",
        "deploy": "gh-pages -d build"
        }
  - make sure you have devDependencies: "gh-pages"!
  
* Create a Github repository and initialize it:
  - git init
  - git remote add origin git@github.com:YOURGITHUB/my-app.git
* deploy the app on Github pages:
  - npm run deploy
* git add .
  git commit -m "Your awesome message"
  git push origin master
