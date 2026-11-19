# Starting the App locally (Dev Environment)

## Prerequisites

* JDK 25
* NODE 24
* a running Docker

Application Commit: dbb150c9fa7989cdca2ba60f62ed5d74b960a2f2

## Cloning the Repo

`git clone https://github.com/GandalfTheJunior/mtg-commander-stats.git`

and

`cd mtg-commander-stats`

## Starting the Database

### Set the Postgres Password

`read -rs "POSTGRES_PASSWORD?Enter Password:" && printf "\n" && export POSTGRES_PASSWORD`

### Start the Database

`docker compose up -d --wait`

## Start the Backend

IMPORTANT: Stay in the same terminal where you set the POSTGRES_PASSWORD.

In the backend folder: `./mvnw spring-boot:run`

## Start the Frontend

Open new Terminal Window, navigate to the frontend folder

### Install Frontend Dependencies

`npm ci`

### start frontend

`npm run dev`

## Open The Application in your browser

Copy the Address you see from Vite in the frontend Terminal into the Browser of your choice.
Create an Account, Log in and Have fun exploring mtg-commander-stats!

## Stop the Application

stop the processes in the frontend and backend terminal with `ctrl + c`
stop the running database with `docker compose stop`
if you want to delete the volume instead use (you will lose all data) `docker compose down -v`