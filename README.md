# Join our [Discord](https://discord.gg/xcjvKPM) channel to be updated.

# Simple SWGOH Arena Tracker
[DiscordChannel](https://discord.gg/xcjvKPM) --my capacity is quite limited, yet you can help each other on this channel

[![](https://c5.patreon.com/external/logo/become_a_patron_button.png)](https://www.patreon.com/iprobedroid)

## Deploy straight to Heroku(24/7 free if a credit card registered)

<!-- [![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://dashboard.heroku.com/new?button-url=https%3A%2F%2Fgithub.com%2Fiprobedroid%2Fswgoh-arena-tracker&template=https%3A%2F%2Fgithub.com%2Fiprobedroid%2Fswgoh-arena-tracker) -->
<!-- [![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy) -->
[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://dashboard.heroku.com/new?button-url=https%3A%2F%2Fgithub.com%2FDV1231%2FccIPD-arena-tracker&template=https%3A%2F%2Fgithub.com%2FDV1231%2FccIPD-arena-tracker)



## Configuration

### Set environment variables:

|Variable Name| Description                             | Notes |
|-------------|-----------------------------------------|------ |
|ARENA_TYPE | `SQUAD` or `FLEET`                 | Required(yet `SQUAD` is by default if not set)|
|DISCORD_WEB_HOOK| Webhook to discord channel.|  Required|
|ALLY_CODES | Comma separated list of ally codes.<br/>Example:<br/>`123456789,123456788,123456999`| Ignored if `ALLY_CODES_URL` present|
|ALLY_CODES_URL| URL to a `json` file with players.<br/> Recommended to use secret github gist like this [example](https://gist.github.com/iprobedroid/603fc48a5ec43afc9e53ee845e91e042/raw)|[How to find discord id.](https://support.discordapp.com/hc/en-us/articles/206346498-Where-can-I-find-my-User-Server-Message-ID-).<br/>Format: `https://gist.github.com/<user_name>/<gist_id>/raw`<br/>Notes:`name` and `discordId` is not required, just set them to an empty string `""`, `userIcon` is for discord emoji(:emoji_code:)  |Recommended|


## Deploy with Heroku steps
### 0. Delete previously created application(if you have one).

### 1. Click the button below.
<!-- [![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://dashboard.heroku.com/new?button-url=https%3A%2F%2Fgithub.com%2Fiprobedroid%2Fswgoh-arena-tracker&template=https%3A%2F%2Fgithub.com%2Fiprobedroid%2Fswgoh-arena-tracker)
 -->
<!-- [![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy) -->
[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://dashboard.heroku.com/new?button-url=https%3A%2F%2Fgithub.com%2FDV1231%2FccIPD-arena-tracker&template=https%3A%2F%2Fgithub.com%2FDV1231%2FccIPD-arena-tracker)


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
Check the application logs if the tracker stops sending messages.

### 6. Activate the resource to run the tracker under the `Resources tab`.
![ScreenShot](assets/activate-worker-resource.png)

### 7. Check logs under `More -> View logs` for any errors.
![ScreenShot](assets/check-logs.png)


### 8. Add a credit card to your profile to get extra free hours for forever free 24/7 hosting.
![ScreenShot](assets/add-credit-card.png)

### 9. Keep only one application and one resource at a time, otherwise you will be charged...

[![](https://c5.patreon.com/external/logo/become_a_patron_button.png)](https://www.patreon.com/iprobedroid)
