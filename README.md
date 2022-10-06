# Portfolio-Backend

### Introduction
Portfolio-Backend is an open source 
 service where you can add data related to personal information, professional career history, personal projects, blog links and ...
### Installation Guide
* Clone this repository [here](https://github.com/Trapeziums/Portfolio-Backend.git).
* The master branch is the most stable branch at any given time, ensure you're working from it.
* Update the necessary variables according to the .env file.
* Install docker and docker-compose depending on your os. [link](https://docs.docker.com/desktop/)
### Usage
* Run the following commands
```sh
- docker network create Portfolio-Backend
- docker volume create db_data
- docker-compose up --build
```
!!! Note Now the project is ready at 127.0.0.1:80
### API Endpoints (User)

!!! Note BaseUrl = https://domain.com/api/v1

| HTTP Verbs | Endpoints | Data | api-key |
| --- | --- | --- | ---|
| POST | /register/ | username , email , password1 , password2 | No
| POST | /login/ | username , password OR email , password | No
| POST | /logout/ | _ | Yes
| POST | /confirm-email/{key:str}/ | key | No
| POST | /password/change/ | old_password , new_password1 , new_password2 |Yes
| POST | /resend_verification_email/ | email | No
| POST | /password_reset/ | email | No
| POST | /password_reset_confirm/{uid}/{token}/ | new_password1 , new_password2 , uid , token | No



### Technologies Used
* [Python](https://nodejs.org/) is dynamically-typed and garbage-collected. It supports multiple programming paradigms, including structured (particularly procedural), object-oriented and functional programming.
* [Django](https://www.expresjs.org/) is a high-level Python web framework that encourages rapid development and clean, pragmatic design. 
* [DjangoRestFrameWork](https://www.mongodb.com/)  (DRF) is a powerful and flexible toolkit for building Web APIs.
* [Docker](https://mongoosejs.com/) is an open platform for developing, shipping, and running applications. Docker enables you to separate your applications from your infrastructure so you can deliver software quickly. 
* [Nginx](https://mongoosejs.com/) pronounced like “engine-ex”, is an open-source web server that, since its initial success as a web server, is now also used as a reverse proxy, HTTP cache, and load balancer.
* [Postgresql](https://mongoosejs.com/) is an advanced, enterprise-class, and open-source relational database system. PostgreSQL supports both SQL (relational) and JSON (non-relational) querying.
* [Git](https://mongoosejs.com/) is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.

* [Celery](https://mongoosejs.com/) is a task queue implementation for Python web applications used to asynchronously execute work outside the HTTP request-response cycle.
* [Redis](https://mongoosejs.com/) is an open source (BSD licensed), in-memory data structure store, used as a database, cache, and message broker. Redis provides data structures …
### License
This project is available for use under the MIT License.