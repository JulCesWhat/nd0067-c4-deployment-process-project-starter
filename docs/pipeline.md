## Pipeline process

1. Github stores the code
2. Circle CI listens for changes to master branch and starts the build when new changes are merged to the branch.
3. After build is succesfull, Circle CI will deploy the changes to S3 and to AWS Elastic Beanstalk.
4. S3 will show the user the index.html so that he can use it.

[Pipeline process AWS](./images/pipeline.png)

