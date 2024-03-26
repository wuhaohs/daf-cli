# Daf Deploy ~ Heroku

Deploy an instance of DAF to Heroku in one click. This example uses an `agent.yaml` file to configure the agent.

This deploment will create some environment variables in your Heroku app. After clicking deploy you will be provided a screen to modify these settings.

#### `APP_URL`

Set this to your base app url. Your default web:did will be based on this when it gets created on first run.

#### `API_KEY`

Used for authorization

#### `SECRET_KEY`

Used for encrypting the database. Please save this or use your own key

#### `AGENT_ENDPOINT`

The url where the agent will be accessible from

## Deploy

Click to launch your agent on Heroku.

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

## Updating deployments

After deploying with the Heroku deploy button you need to link your local repo with heroku. Ensure you have the heroku CLI installed and authenticate.

```bash
$ heroku login
$ git remote add APPNAME.heroku https://git.heroku.com/APPNAME.git
$ git push APPNAME.heroku master
```

## Local Deploy

This will create a local instance. Run ngrok or https local server for web:did functionality

```bash
$ yarn install
$ yarn dev
```
