# Getting Started with Create React App Reference

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Using to start a new React project

1. Run `git clone git@github.com:williamwdev/react-boilerplate.git new-project-name`
2. Run `npm install` to install dependencies
3. Run `npm start`
4. Create a mew rep on Github
5. Run `git remote set-url` to check current origin & Run `git remote set-url origin git@github.com:williamwdev/project-name`
6. Run `git add .` & `git commit -m 'initial commit'` & `git push` 

## Building for production and deploying on Vercel

1. Run `npm run build` to create optimized files to deploy
2. Set up and install [Vercel](https://vercel.com/) and run `vercel --version`
3. Run `vercel login` and run `vercel` to deploy with the CLI
4. Run `touch ./vercel.json` to create file for custom configurations in the root directory of project
```javascript
{
  "version": 2,
  "routes": [
      { "handle": "filesystem" },
      { "src": "/.*", "dest": "/index.html" }
  ]
}
```
5. Add custom scripts for deploying in package.json file
```javascript
"scripts": {
...
"predeploy": "npm run build",
"deploy": "vercel --prod"
}
```
6. Run `npm run deploy` to deploy new build
7. Run `vercel alias [previous-deploy-url] [alias]`

## Fresh Set up

1. Make sure to have the most current version of [Node](https://nodejs.org/en/)
2. Run `node --version` and `npm --version`
3. Run `npx create-react-app name-of-project`
4. Run `npm install` to install all dependencies
5. Run `rm ./src/serviceWorker.js ./src/App.css ./src/logo.svg`
6. Update contents of `./src/App.js` as follows:
``` javascript
import React from 'react';

function App() {
  return (
    <main className='App'>
      <h1>New Project</h1>
    </main>
  );
}

export default App;
```
7. Update contents of `./src/index.js` as follows:
``` javascript
import React from 'react';
import ReactDOM from 'react-dom';
import App from './App';
import './index.css';

ReactDOM.render(<App />, document.getElementById('root'));
```

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.\
You will also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: [https://facebook.github.io/create-react-app/docs/code-splitting](https://facebook.github.io/create-react-app/docs/code-splitting)

### Analyzing the Bundle Size

This section has moved here: [https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size](https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size)

### Making a Progressive Web App

This section has moved here: [https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app)

### Advanced Configuration

This section has moved here: [https://facebook.github.io/create-react-app/docs/advanced-configuration](https://facebook.github.io/create-react-app/docs/advanced-configuration)

### Deployment

This section has moved here: [https://facebook.github.io/create-react-app/docs/deployment](https://facebook.github.io/create-react-app/docs/deployment)

### `npm run build` fails to minify

This section has moved here: [https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)
