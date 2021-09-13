# Pipeline Process

CircleCI is used to perform CI/CD pipeline.

## Configuration For CircleCI

Separated the workflow in frontend and backend.

1 Frontend:  
    - node/install  
    - checkout  
    - aws-cli/setup  
    - Front-End Install  
    - FrontEnd Build    
    - FrontEnd Deploy  

2 Backend.
    - BackEnd Install
    - BackEnd Build
    - BackEnd Deploy

## Schema

![](../screenshots/pipeline.png)
