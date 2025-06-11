# mma-mini-app
Resilient Multi-messenger astronomy application

## Requirements
To run the mini app, Docker must be installed.

## Configuration
The mini-app requires Octopus and ProxyStore authentication information in order to execute. These configuration variables are set within a `.env` file.
[.env.template](.env.template) provides an example of which variables must be set.

`.env`
```
OCTOPUS_AWS_ACCESS_KEY_ID=<Octopus access key>
OCTOPUS_AWS_SECRET_ACCESS_KEY=<Octopus AWS access secret>
OCTOPUS_BOOTSTRAP_SERVERS=<Octopus Bootstrap servers>
PROXYSTORE_GLOBUS_CLIENT_ID=<Globus client ID to authenticate user to ProxyStore>
PROXYSTORE_GLOBUS_CLIENT_SECRET=<Globus client secret to authentication user to ProxyStore>
```

## Build and execute

Docker-compose is used to build and run the mini-app. This can be achieved through the following command:

```
docker-compose up
```