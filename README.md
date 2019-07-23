
If creating a new heroku project

 - `heroku create myapp --buildpack https://github.com/khanduri/heroku-gcp-credentials-buildpack.git`

If adding buildpack to an existing heroku project

 - `heroku buildpacks:set -a [APP_NAME] https://github.com/khanduri/heroku-gcp-credentials-buildpack.git`

Setting env variables

 - `heroku config:set -a [APP_NAME] GCS_CREDENTIALS_JSON_STR="$(< path/to/creds.json)" GOOGLE_APPLICATION_CREDENTIALS=google-credentials.json`
