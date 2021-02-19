# A Basic Data Ingestor API
## Written in node.js

A very simple node.js app using express and mongoDB.

POST requests to /data are saved in mongoDB saves the request body inside a JSON object.

GET requests to /data and / with no query parameters can be used to get list of all objects.

Querying specific data by id is permitted, but not tested yet.

Showcases simple node.js app structure and mongoose ODM/backend mongoDB connectivity.

Deployable in heroku, however the config var MONGO_CONN_STRING needs to be set.

For local deployments, a project.properties file can be added at root path:

    [main]
    MONGO_CONN_STRING=<connection string>
