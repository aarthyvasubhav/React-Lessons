# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

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

**Note: this is a one-way operation. Once you `eject`, you can't go back!**

If you aren't satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you're on your own.

You don't have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn't feel obligated to use this feature. However we understand that this tool wouldn't be useful if you couldn't customize it when you are ready for it.

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


Points to remember:<footer></footer> - default html element starts with small letter<Footer /> - custom HTML element should be in the capital first letter, it is pre-defined to differentiate

React properties:
If we create an i]html input elements we can pass lots of attributes ex:
<input type="text" placeholder="enter your first name" value ="Aarthy" />
Here placeholder and values are attributes
In React we can create our own/custom attributes for custom HTML tags
for example:<Card name="Aarthy" tel="3289u84u2" />
Benefits of the above:If we have a card saying the person's name img and telephone number instead of creating 1000 cards use the above method and follow the code as an example.
In the below code function props <function Card(props){<h2>{props.name}</h2>} is  being passed props or any word passes the properties which we give in custom HTML tag while rendering("<Card name="Beyone" />
import React from "react";import ReactDOM from "react-dom";
const root = ReactDOM.createRoot(document.getElementById('root'));
function Card(props){
    return <div>        <h2>{props.name}</h2>    </div>}root.render(    <div> <h1>My contacts</h1> <Card name="Beyonce"/> </div>)





FULL CODE
HTML PAGE:
<!DOCTYPE html><html lang="en">  <head>    <title>React Properties</title>  </head>  <body>    <div id="root"></div>    <script src="../src/index.js" type="text/jsx" ></script>  </body></html>

Index.js page
import React from "react";import ReactDOM from "react-dom";
const root = ReactDOM.createRoot(document.getElementById('root'));
function Card(props){
    return <div>        <h2>{props.name}</h2>        <img src={props.img} alt="avatar_img" />        <p>{props.tel}</p>        <p>{props.email}</p>    </div>}root.render(    <div> <h1>My contacts</h1> <Card name="Beyonce" img="https://blackhistorywall.files.wordpress.com/2010/02/picture-device-independent-bitmap-119.jpg"    tel = "+123 456 789" email ="b@beyonce.com" />
<Card name="Jack Bauer" img="https://pbs.twimg.com/profile_images/625247595825246208/X3XLea04_400x400.jpg"    tel = "+123 456 789" email ="b@beyonce.com" />
<Card name="Chuck Norris" img="https://i.pinimg.com/originals/e3/94/47/e39447de921955826b1e498ccf9a39af.png"    tel = "+123 456 789" email ="b@beyonce.com" /> </div>)But in CUSTOM HTML TAG Element className property does not work -because everything it sees as custom propert insteaed of seeing it as html attribute.
Full code with 
Git code commited.
