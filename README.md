# GraphQL + React Event Booking API

This code belongs to a tutorial series: [https://github.com/academind/yt-graphql-react-event-booking-api.git](https://github.com/academind/yt-graphql-react-event-booking-api.git)

# Usage

## Development

You can run this example application inside Docker contaniers. To do that you need:

* Install Docker.
* Install Docker-Compose.
* Install [dip](https://github.com/bibendi/dip).
* [Integrate](https://github.com/bibendi/dip#integration-with-shell) dip into you ZSH console.
* Provision backend application: `provision`.
* Start Node server: `yarn start`, or `yarn start:dev`, or `yarn start:debug`.
* Open another terminal and change current directory to `frontend`.
* Provision frontend application: `provision`.
* Start React server: `yarn start`.
* Open in browser https://localhost:3000

## Debug

You can debug this code through VS Code. To do that you need^

* Create file `.vscode/launch.json` with below contents:

  ```json
  {
    // Use IntelliSense to learn about possible attributes.
    // Hover to view descriptions of existing attributes.
    // For more information, visit: https://go.microsoft.com/fwlink/?linkid=830387
    "version": "0.2.0",
    "configurations": [
      {
        "type": "node",
        "request": "attach",
        "name": "Docker: Attach to Node",
        "port": 9229,
        "address": "localhost",
        "localRoot": "${workspaceFolder}/",
        "remoteRoot": "/app/",
        "protocol": "inspector"
      }
    ]
  }
  ```

* Run backend application: `yarn start`.
* F5 -> Start debugging in VS Code.
