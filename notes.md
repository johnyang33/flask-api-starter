## Let's create a CRUD Rest API in Python, using:

    1. Flask (Python web framework)
    2. SQLAlchemy (ORM)
    3. Postgres (database)
    4. Docker (containerization)
    5. Docker Compose (to run the application and the database in containers)


## To run the Postgres container, type:

``docker compose up -d flask_db``

The -d flag is to run the container in detached mode, so it will run in the background.

To check if the container is running, type:
p
``docker compose logs``

If the last line is LOG: database system is ready to accept connections, 
it means that the container is running and the Postgres server is ready to accept connections.

To show all the containers (running and stopped ones) type:

``docker ps -a``

Now, to test the db connection, we can use any tool we want. Personally, I use TablePlus.

##  Build and run the Flask application 

``docker compose build``

Now, to check if the image has been built successfully, type:

``docker images``

## Run the flask_app service

``docker compose up flask_app``

## Test the application

``localhost:4000/test``

