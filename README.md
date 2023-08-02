# Buildpack GitHub Access Token

Get GitHub API's Access Token

## How to local develop

Create the necessary files with the following commands.

```
mkdir cache env
touch env/{GITHUB_USER,GITHUB_ORG,GITHUB_REPO,GITHUB_APP_ID,GITHUB_APP_PRIVATE_KEY_BASE64}
```

Run build.

```
docker run --platform linux/x86_64 -i -v .:/app -w /app heroku/heroku:20-build ./bin/compile /app /app/cache /app/env
```
