# Project Title - Deploy a high-availability web app using CloudFormation
This folder provides the code for the "Deploy a high-availability web app using CloudFormation" project. This folder contains the following files:


## infrastructure.yml
A CloudFormation code using this YAML template for building the cloud infrastructure, as required for the project. 

## parameters.json
A JSON file for increasing the generic nature of the YAML code. For example, the JSON file contains a "ParameterKey" as "EnvironmentName" and "ParameterValue" as "UdacityProject". 

In YAML code, the `${EnvironmentName}` would be substituted with `UdacityProject` accordingly.

## update.sh and create.sh 
Two sh files for simplify the deployment of the cloudformation script the following parameters are required 
- aws profile (use default if non is created)
- stack name
- template body 
- parameters body 


### usage sample:  

```bash 
./create.sh udacity-aws-profile infra infrastructure.yml parameters.json
```

```bash 
./update.sh udacity-aws-profile infra infrastructure.yml parameters.json
```

## infrastructure-diagram.png
The Diagram for the infrasctructure implemented

## index.html
HTML file to be add to the S3 bucket 

## Requirements to run project 

In this project the following are assume 
- An S3 bucket with the index.html in it is already created , the **S3 Name** can be updated in the parameters.json file.
- The user is in the us-east-1 aws region


## Temporary Working URL of review 

[http://infra-webse-fcv86iidigu6-1558822400.us-east-1.elb.amazonaws.com](http://infra-webse-fcv86iidigu6-1558822400.us-east-1.elb.amazonaws.com)