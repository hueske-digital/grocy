# Grocy

This repository contains [Grocy](https://grocy.info/).

## Requirements

Make sure that the [nginx reverse proxy](https://gitlab.com/hueske-digital/services/proxy) is already set up and started.

## Setup instructions

Clone the code to your server:<br>
```
git clone git@gitlab.com:hueske-digital/services/grocy.git ~/services/grocy
```

Create environment file and fill up with your values:<br>
```
cd ~/services/smarthome && cp .env.example .env && vim .env
```

Pull images and start the docker compose file:<br>
```
docker compose up -d
```

While waiting you can create a host in your nginx proxy manager which points to `grocy-app-1` with port `80`.
