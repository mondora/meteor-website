[![Code Climate](https://codeclimate.com/github/mondora/mondora-website-back.png)](https://codeclimate.com/github/mondora/mondora-website-back)

# Mondora Website Back

This is the repository of of the mondora website backend. The source code for
the frontend can be found at
[mondora/mondora-website-front](https://github.com/mondora/mondora-website-front).


## Development environment setup

If you don't have `meteor` installed, you can install it following instructions
at [meteor.com/install](https://www.meteor.com/install).

```sh
git clone https://github.com/mondora/mondora-website-back.git
cd mondora-website-back
meteor
```
> Due to a STRAVA API call at startup, to spawn the app without blocking exceptions you must set the following environment vars:
>
> **STRAVA_API_URL** = https://www.strava.com/api/v3/clubs/148440/activities
> 
> **STRAVA_REFRESH_INTERVAL** = 3600000
>
> Although the server is up, it will log a warning into console (401 - api token error) whenever the refresh interval expires.
> The **STRAVA_API_TOKEN** env var is required if you want to change/improve the STRAVA service implementation.
