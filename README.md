# SWADE_CS
Savage Worlds Adventurer Edition Dynamic Character sheet

This sheet will use a database created using [Airtable](https://airtable.com/)

Initially it will just supply some quick lookup stuff for the spells, skills, and edges. Eventually I want to turn it in to a full character sheet that will track the characters abilities - something like what D&D Beyond did with theirs.

### 12/7/2019
Airtable makes a Node library, but they don't tell me how to wire it in easily. Since I don't know Webpack or Browerify, I'd rather not try to use it. However, the Airtable API does include the curl commands for accessing the DB. This gives me the urls that I need to do the get and post commands. I need to be sure to add the key at the end. example:

    curl "https://api.airtable.com/v0/YOUR_BASE_ID/Powers?maxRecords=3&view=Grid%20view" \
    -H "Authorization: Bearer YOUR_API_KEY"
              |
              V
     https://api.airtable.com/v0/YOUR_BASE_ID/Powers?maxRecords=3&view=Grid%20view&api_key=YOUR_API_KEY}`;

(Found this trick in the comments of https://css-tricks.com/use-airtable-front-end-developer/.)

--------------------
# Other things to know

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.<br />
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br />
You will also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.<br />
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.<br />
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br />
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

This section has moved here: https://facebook.github.io/create-react-app/docs/code-splitting

### Analyzing the Bundle Size

This section has moved here: https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size

### Making a Progressive Web App

This section has moved here: https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app

### Advanced Configuration

This section has moved here: https://facebook.github.io/create-react-app/docs/advanced-configuration

### Deployment

This section has moved here: https://facebook.github.io/create-react-app/docs/deployment

### `npm run build` fails to minify

This section has moved here: https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify
