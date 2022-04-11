# Backend Assessment
A dockerized uptime monitoring RESTful API server that allows authenticated users to monitor URLs, and get detailed uptime reports about their availability, average response time, and total uptime/downtime.

## Overview
- Signup with email verification.
- CRUD operations for URL checks (`GET`, `PUT` and `DELETE` can be called only by the user user who created the check).
- Authenticated users can get detailed uptime reports about their URLs availability, average response time, and total uptime/downtime.
- Authenticated users can group their checks by tags and get reports by tag.
- Stateless authenication using JWT.
- APIs consume and produce `application/json`.

## Setup

### Installing locally
- `npm install`
- Create a new database named bostaDB on MongoDB and change the `.env` file with the new connections details, (OR you can work with the current database)
-  `npm run start`

### Installing the Docker image
- Download the repo
- cd to the project directory
- Run in terminal `docker-compose -f docker-compose.yml up`
