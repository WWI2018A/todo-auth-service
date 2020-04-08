# Auth-Service

## Keycloak for Todo
This repo contains a docker-compose.yml file for creating an standalone Keycloak environment for the todo application  
The project emerged due to our studies at the DHBW Stuttgart

### Requirements
To run this you will need to have docker, docker-compose installed on your machine

### How to Run

```bash
  cd config/
  docker-compose up -d
```

### Environment variables

 - `KEYCLOAK_USER` : name of the inital admin account
 - `KEYCLOAK_PASSWORD`: password of the initial admin account
 - `KEYCLOAK_FRONTEND_URL`: The url of the frontend (Example: `sub.example.com/api/v1/auth`)
 - `DB_VENDOR`: name of the database vendor
 - `DB_ADDR`: address of the database (url or ip)
 - `DB_USER`: user of the database 
 - `DB_PASSWORD`: password of the database user
 - `PROXY_ADDRESS_FORWARDING`: set this to true, if you want to run Keycloak behind a reverse proxy

