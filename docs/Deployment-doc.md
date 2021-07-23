## Infrastructure

### Develop Env
1. Github repository to store the code.
2. Circle CI for CI/CD

### Production ENV
1. Postgress database is available with AWS RDS.
2. S3 to store the files uploaded in the project.
3. The UI is hosted in S3.
4. The Api server is avaiable with AWS Elastic Beanstalk.


## Pipeline process
1. The application code is sent to Github
2. After merging changes to master branch, the code is sent to Circle CI
3. Circle CI builds the project and deploys it to AWS
4. AWS allows to host the server and displays it to the users.


## App dependencies
- NodeJS
- npm

### Frontend
- Angular 
- Typescript

### Backend
- ExpressJS
- Sequelize
- AWS-SDK
- S3 bucket

### Database
- Postgres database with AWS RDS

### Deployment
- AWS CLI
- EB CLI

### Environment variables

```
POSTGRES_USERNAME, POSTGRES_PASSWORD, 
POSTGRES_DB, POSTGRES_PORT, POSTGRES_HOST, 
PORT, AWS_REGION, AWS_PROFILE, 
AWS_BUCKET, URL, JWT_SECRET, 
AWS_ACCESS_KEY_ID, AWS_SECRET_ACCESS_KEY
```
