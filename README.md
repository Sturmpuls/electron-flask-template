# A template to easily deploy flask apps with Electron

## Resources
* based on [electron-flask](https://github.com/matbloch/electron-flask)

### Dependencies
* [Node.js](https://nodejs.org/en/)
* [Python](https://www.python.org/)

## Setup
1. Install Node.js
1. Install Python
1. `git clone https://github.com/Sturmpuls/electron-flask-template.git`
1. `cd electron-flask-template`
1. `npm install`
1. `pip install virtualenv`
1. `virtualenv env --copies --clear`
1. `source env/Scripts/activate`
1. `pip install -r requirements.txt`

# Run the Application
## Start Electron + Flask
`source env/Scripts/activate`
`npm start`

## Start Flask
`source env/Scripts/activate`
`flask run`

## Compile Electron + Flask
`source env/Scripts/activate`
`npm package`

## Compile Flask
`source env/Scripts/activate`
`npm package-python`

## Settings
Flask
* ./config.py - can be used for development, will be committed.
* ./config_local.py - should be used for production, will NOT be committed.
Environment
* /.flaskenv - can be used for development, will be committed.
* /.env - should be used for production, will NOT be committed. Variables set here are used over those set in .flaskenv.
