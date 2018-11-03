# nyt-search
MERN Stack Implementation of a New York Times News API Search App

pseudo-code of the steps needed to implement the app:
* import the necessary npm packages for the project: axios (or request), express, mongoose, if-env, dotenv, nodemon, concurrently, path, etc.
* set up the front-end for the project inside the project root directory using `crate-react-app client`
* while the above completes, create the models directory in the root folder of the project and set up the Article mongoose schema inside it
* create the controllers folder inside the project root folder and set up articlesController with the CRUD methods necessary for article manipulation in our app
* create the routes folder inside the project root folder and set up api routes that will leverage the articlesController to perform all the CRUD operations associated with articles in our app
* create a server.js file inside the project root folder, import the necessary npm packages in it, set up the runtime configuration for the express server and then set up the code to start the back-end server when server.js is executed
* inside client/public/index.html, import bootstrap, jquery and all the necessary libraries and files to use in the front end
* create the pages/ directory inside client/src and set up these components:
	1. Search - display the form in a page that the user can input filtering info to find the articles they are looking for
	2. Results - the page that shows the results of the search done previously. this component will leverage the ResultListing component inside src/components to list out the articles in the search results
	3. Saved - displays the articles saved by the user from the Results view. this component will alsove leverage the ResultListing component to list out the articles that were save previously by the user. the only that that will change is the button. While this was labellled 'Save' in the Results view, in the Saved view it will be labelled 'Delete' and will delete the saved articled from the db when the user clicks it