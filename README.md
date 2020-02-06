# React to To Do List

## Features:
* add new items to your to do list
* mark items as done
* remove items from your list

## Dependencies
    "axios": "^0.19.2",
    "dom": "0.0.3",
    "gh-pages": "^2.2.0",
    "react-dom": "^16.12.0",
    "react-router": "^5.1.2",
    "uuid": "^3.4.0"
    
 ## Commands for deployment of your React App on GitHub Pages:
 1- First create a repository named my-app using create-react-app.

npm init react-app my-app

2- We need to install GitHub Pages package as a dev-dependency.

cd my-app
npm install gh-pages --save-dev

3- Add properties to package.json file.

The first property we need to add at the top level homepage second we will define this as a string and the value will be "http://{username}.github.io/{repo-name}" {username} is your GitHub username, and {repo-name} is the name of the GitHub repository you created it will look like this :

"homepage": "http://yuribenjamin.github.io/my-app"

Second in the existing scripts property we to need to add predeploy and deploy.

"scripts": {
//...
"predeploy": "npm run build",
"deploy": "gh-pages -d build"
}

package.json example

4- Create a Github repository and initialize it and add it as a remote in your local git repository.

Now, create a remote GitHub repository with your app name and go back initialize this
git init
add it as remote
git remote add origin git@github.com:Yuribenjamin/my-app.git

5- Now deploy it to GitHub Pages.

just run the following command :

npm run deploy

successful build

this command will create a branch named gh-pages this branch host your app, and homepage property you created in package.json file hold your link for a live preview, or you can open the branch setting scroll down to GitHub Pages section you will find this:
Your site is puplished

Visit deployed app

6- commit and push your commit to GitHub. Optionally

git add .
git commit -m "Your awesome message"
git push -u origin master
