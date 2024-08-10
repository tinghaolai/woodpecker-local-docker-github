# Local docker and Github

1. Github OAuth Apps setting

generate new OAuth Apps for woodpecker

* Homepage URL: http://localhost:8000
* Authorization callback URL: http://localhost:8000/authorize


2. fill
.env
```
WOODPECKER_HOST=http://localhost:8000
WOODPECKER_AGENT_SECRET=example-secret
WOODPECKER_GITHUB_CLIENT=example-client
WOODPECKER_GITHUB_SECRET=example-secret
```

* WOODPECKER_AGENT_SECRET: any string
* WOODPECKER_GITHUB_CLIENT: Github client id (OAuth Apps)
* WOODPECKER_GITHUB_SECRET: Github client secret (OAuth Apps)

3. `docker-compose up -d` and open http://localhost:8000


