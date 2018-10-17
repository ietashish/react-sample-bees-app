# react-sample-bees-app
A React Sample Application used for SPA demos

# What does the app provide
1. The app is a single page application with multiple views. 
2. The following piece of code is already implemented in the app (inside `src/index.js`) which is responsible for triggering view.
```javascript
   if (typeof adobe != 'undefined' && adobe.target && typeof adobe.target.triggerView === 'function') {
            let viewName = window.location.hash;
            viewName = viewName.substring(2);

            console.log("Triggering view: " + viewName);
            adobe.target.triggerView(viewName);
    }
```

# How to get the app running

### Clone the repo : 
`git clone git@git.corp.adobe.com:ashishg/demostore.git`

### Include your org's at.js : 
1. Download at.js for SPA from "Setup > Implementation > “Download at.js for SPA"
2. Replace the at.js in `js` directory with the downloaded one.

### Install npm dependencies : 
1. cd in react-sample-bees-app
2. `npm install`
3. `npm run build`
4. `npm run start`


### Go to 
The app will start at http://localhost:3000/
