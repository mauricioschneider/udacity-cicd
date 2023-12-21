# Udagram Infrastructure

![Udagram](https://github.com/mauricioschneider/udacity-cicd/blob/master/docs/images/udagram-architecture-diagram.png?raw=true)

As shown in the diagram above, the Udagram application has three components: front-end, API, and database.

## Front-end

Udagram's front-end is an Angular application. It production, it's stored in an Amazon S3 bucket configured to serve its content as static website.

![Udagram](https://github.com/mauricioschneider/udacity-cicd/blob/master/docs/images/aws-s3-bucket.png?raw=true)

## API

The Udagram API is an express application. It uses sequelize as ORM to handle the connection with the Postgres database. In production, it's stored in an Amazon Elastic Beanstalk application environment.

![Udagram](https://github.com/mauricioschneider/udacity-cicd/blob/master/docs/images/aws-eb.png?raw=true)

## Database

Postgres is the database engine used by Udagram. It's in charge of persisting data related to users and their respective feeds. In production, is ran in Amazon RDS.

![Udagram](https://github.com/mauricioschneider/udacity-cicd/blob/master/docs/images/aws-rds.png?raw=true)