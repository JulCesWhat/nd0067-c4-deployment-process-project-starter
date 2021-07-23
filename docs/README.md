## Infrastructure

[Application Link](http://capivara-test-1.s3.amazonaws.com/index.html)

1. Github
2. Circle CI
3. Postgress with AWS RDS
4. AWS S3
5. AWS Elastic Beanstalk

The user goes to the page. The user interacts with the BE that is hosted in Elastic Beanstalk. The application stores the users in postgres db. Once the user is logged in, the user can create posts and upload the pictures in s3.

[Infrastructure AWS](./images/infrastructure.png)


## Pipeline process
1. Github stores the code
2. Circle CI listens for changes to master branch and starts the build when new changes are merged to the branch.
3. After build is succesfull, Circle CI will deploy the changes to S3 and to AWS Elastic Beanstalk.
4. S3 will show the user the index.html so that he can use it.

[Pipeline process AWS](./images/pipeline.png)

### Environment variables

```
POSTGRES_USERNAME
POSTGRES_PASSWORD, 
POSTGRES_DB
POSTGRES_PORT
POSTGRES_HOST, 
PORT
AWS_REGION
AWS_PROFILE, 
AWS_BUCKET
URL
JWT_SECRET, 
AWS_ACCESS_KEY_ID,
AWS_SECRET_ACCESS_KEY
```


