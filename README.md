# React to To Do List

## Features:
* add new items to your to do list
* mark items as done
* remove items from your list

## Dependencies
    "axios": "^0.19.2",
    "gh-pages": "^2.2.0",
    "react-dom": "^16.12.0",
    "react-router": "^5.1.2",
    "uuid": "^3.4.0"
    
 ## Commands for deployment of your React App on GitHub Pages:
 ### 1- Create a repository named my-app using create-react-app.

    npm init react-app my-app

### 2- Install GitHub Pages package as a dev-dependency.

    cd my-app
    npm install gh-pages --save-dev

### 3- Add properties to package.json file.

    - "homepage": "http://{username}.github.io/{repo-name}",     /DO NOT FORGET THE COMA  " ," after!/
    -  in "scripts" add predeploy and deploy:
            "scripts": {
            //...
            "predeploy": "npm run build",
            "deploy": "gh-pages -d build"
            }


### 4- Create a Github repository and initialize it and add it as a remote in your local git repository.

    git init
    git remote add origin git@github.com:{USERNAME}/my-app.git

### 5- Deploy it to GitHub Pages.
 
    npm run deploy

### 6- Commit and push your commit to GitHub.

    git add .
    git commit -m "Your awesome message"
    git push -u origin master
