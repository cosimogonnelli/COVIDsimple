## FULL-STACK PROJECT - COVIDsimple - 

### OVERVIEW 

Our web-app provides tools for COVID-19 data visualization and for browsing relevant COVID-19 news.

### FEATURES

1. Data Visualization for US COVID data
	* Produces a heat map of US states indicating state-by-state trends
	* Allows user to select between a variety of data display modes and statistics
	* Allows user to smoothly change between visualizations of the data from any dates since the outbreak began  
2. Allow users to perform comparisons between states 
	* Allow users to view all of a state's historical data for any particular statistic through a variety of available graph types
	* Allow multiple states’ data to be overlaid on same chart for comparison.
3. Present articles or news relevant to COVID
	* Provides 2 sets of articles: latest CDC and WHO news, and user rated articles
	* Allow users to sort latest and rated article sets by source, date, and name (asc, desc)
	* Allow users to filter articles by source
	* Allow users to preview the latest articles before navigating to them

### Tutorials Used
1. Full Stack React/Express with Postgres: https://www.youtube.com/watch?v=Z4jCvpSROp8
2. Full Stack React/Express: https://www.youtube.com/watch?v=7CqJlxBYj-M
3. React-Strap Sample Code for understanding how to implement their components: https://reactstrap.github.io/
4. Basic 404 redirecting using examples here: https://www.youtube.com/watch?v=c5ODpAPrB74

### Stack Technologies
1. React frontend
2. Reactstrap and Bootstrap4 for layout
3. CSS styling
4. Express and Node.js backend
5. PostgresSQL databases hosted in Google Cloud and on Heroku

### Packages integrated
#### Client
1. Packages to support graphing: d3, re-charts, react-simple-maps
2. Packages to support forms associated with graphs: react-datepicker, react-input-slider, react-tooltip, moment, jquery
3. Packages to help with news: react-html-parser
4. General purpose packages used: typescript
#### Server
1. Packages to support external apis; axios, rss-parser
2. Packages to support general infrastructure: pg, dotenv, cors, cookie-parser, body-parser

### Install Insructions for Developers
1. Please note that the server expects to connect to one of our hosted databases, or another PG instance which you may use environment variables to specify. See the create_table.sql file for context on db structure
2. To configure connection to postgres database, an environment variable file (.env) should include (with appropriate values assigned of course):
	- DB_USER=
	- DB_NAME=
	- DB_HOST=
	- DB_PWD=
	- PG_PORT=
3. Dev install: 
   * checkout code
   * cd COVIDsimple/
   * run `npm install && npm --prefix ./client install ./client`
   * run `npm start` 
4. At this point both the client and server should be running
5. If you are not immediately redirected, navigate to http://localhost:3000/
6. To just excercise the server api endpoints navigate to http://localhost:5000 and the appropriate end point
### Production app
To view the app in it's production build, visit <https://covidsimple.herokuapp.com>

