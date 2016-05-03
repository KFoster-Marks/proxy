# CorsProxy

*Needed a way for students to get around CORS issues for front-end only projects?*
Just set `apiServerHost` as a Heroku config variable, and have students point their API request to the Heroku-app instead of the API that doesn't support CORS.

## Setup
  - Set the config var: `heroku config:set apiServerHost=API_TO_PROXY` replace `API_TO_PROXY` with the API you want to proxy. E.g.: `heroku config:set apiServerHost=http://www.omdbapi.com`

## Usage
  - Make requests to: `https://YOUR_APP_NAME.herokuapp.com/?t=the+matrix&y=&plot=short&r=json`
