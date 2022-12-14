# Spring Boot and React Docker-compose example

- Put Dockerfile(s) into appropriate dir
- Update `context` in docker-compose.yaml if needed
- Export secrets as env variables prior to run (POSTGRES_PASSWORD, AUCTION_APP_JWTSECRET)

```
# build and start services locally

docker-compose up -d --build
```

## Deploy to EC2 using GitHub Actions

- Add self-hosted runner on GitHub repo as described [here](https://docs.github.com/en/actions/hosting-your-own-runners/adding-self-hosted-runners)
- Create GitHub Actions Worflow using [example yaml](.github/workflows/deploy.yml)