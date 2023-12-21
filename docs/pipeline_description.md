# Pipeline Description

Udagram uses CircleCI to manage its CI/CD pipeline. An integration between Github and CircleCI allows the pipeline to be automatically triggered with any code pushed to the repository.

![Udagram](https://github.com/mauricioschneider/udacity-cicd/blob/master/docs/images/circleci-pipeline-diagram.png?raw=true)

As shown in the diagram above, the Udagram application has three components: front-end, API, and database.

## Build

During this step, the CircleCI environment is prepared by installing all dependencies necessary to build Udagram. The specific steps can be seen below.

![Udagram](https://github.com/mauricioschneider/udacity-cicd/blob/master/docs/images/circleci-build?raw=true)

## Approve

Once the build process is ready, a manual approval is required to proceed with the deployment

![Udagram](https://github.com/mauricioschneider/udacity-cicd/blob/master/docs/images/circleci-approve?raw=true)

## Deploy

As soon as the approval is provided by an organization user in CircleCI, the deployment process takes place. The steps involved in this process can be seen below.

![Udagram](https://github.com/mauricioschneider/udacity-cicd/blob/master/docs/images/circleci-deploy?raw=true)

## Environment Variables

In order for the pipeline to work as intended, a few environment variables need to be setup in the CircleCI project:

![Udagram](https://github.com/mauricioschneider/udacity-cicd/blob/master/docs/images/circleci-env?raw=true)