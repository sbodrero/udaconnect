# Pipeline Process

CircleCI is used to perform CI/CD pipeline.

## Configuration For CircleCI

1. ASeparated the workflow in frontend and backend.
2. Then we install them and checkout.  See below which is in config.yml file:
    - node/install
    - node/install-yarn
    - checkout
    - aws-cli/setup
3. Then we would install, build, and deploy on both parts: frontend and backend.  The following is in order so it would run smoothly.
    - FrontEnd Install
    - BackEnd Install
    - FrontEnd Build
    - BackEnd Build
    - BackEnd Deploy (need to be this first before FrontEnd Deploy since FrontEnd is depending on API)
    - FrontEnd Deploy

## Schema

![](../screenshots/pipeline.png)
