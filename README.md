# Simple SWGOH Arena Tracker

## Deploy straight to Heroku(24/7 free if a credit card registered)

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

## Configuration

### Set environment variables:

ALLY_CODES - comma separated list of ally codes

ARENA_TYPE - `SQUAD`/`FLEET`

DISCORD_WEB_HOOK - web hook to discord channel

GAME_CLIENT_VERSION - not required, but in case of new game updates can crash the tracker(current version is 0.16.1)

## Deploy with Heroku steps
### 0. Delete previously created application(if you have one).

### 1. Click the button below.
[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)
### 2. Create the application with a unique name and press `Deploy app` button.
![ScreenShot](assets/create-app.png)

### 3. Once deployed press `Manage App` button.
![ScreenShot](assets/app-deployed.png)

### 4. Go to settings tab.
![ScreenShot](assets/go-to-settings-tab.png)

### 5. Press `Reveal Config Vars` button and set environment variables.
![ScreenShot](assets/set-env-variables.png)

Ally codes is a comma-separated string(like: 123456789,125456189 ...).

You will need to create a Discord web hook in the channel of choice.
Fill the `DISCORD_WEB_HOOK` with the that unique url.

Choose your arena type - `SQUAD` or `FLEET`.

`GAME_CLIENT_VERSION` is not required at first but will help to fix connection
issues when the game client will be updated again(happens from time to time).
Check the application logs if the tracker stops sending messages.

### 6. Activate the resource to run the tracker under the `Resources tab`.
![ScreenShot](assets/activate-worker-resource.png)

### 7. Check logs under `More -> View logs` for any errors.
![ScreenShot](assets/check-logs.png)


### 8. Add credit card to your profile to get extra free hours for full month free 24/7 hosting.
![ScreenShot](assets/add-credit-card.png)

### 9. Keep only one application and one resource at a time, otherwise you will be charged...

