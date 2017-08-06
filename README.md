[![Code Climate](https://codeclimate.com/github/mondora/mondora-website-back.png)](https://codeclimate.com/github/mondora/mondora-website-back)

# Mondora Website Back

This is the repository of of the mondora website backend. The source code for
the frontend can be found at
[mondora/mondora-website-front](https://github.com/mondora/mondora-website-front).


## Development environment setup

If you don't have `meteor` installed, you can install it following instructions
at [meteor.com/install](https://www.meteor.com/install).

### Strava setup

Create an application at [strava.com/settings/api](https://www.strava.com/settings/api) and make note of your `access_token`.
In order to start the application you need to set the following environment variables:

* `STRAVA_API_URL`=`https://www.strava.com/api/v3/athlete/activities`
* `STRAVA_API_TOKEN`=`your_access_token`
* `STRAVA_REFRESH_INTERVAL`=`60000`

For more information about the Strava API please refer to the [Strava API Reference](http://strava.github.io/api/)

Example usage:

```sh
git clone https://github.com/mondora/mondora-website-back.git
cd mondora-website-back
STRAVA_API_URL='https://www.strava.com/api/v3/athlete/activities' STRAVA_API_TOKEN='your_access_token' STRAVA_REFRESH_INTERVAL='60000' meteor
```
