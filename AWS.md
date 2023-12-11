# Amazon Web Services

## TAGS

* all projects should have a tag
  * apt-podcasts - aptpodcaststudios.com
  * apt-worldwide - aptww.org
  * trac-subs - carriage reporting
  * **add any new projects to this list**
* Add a tag to EVERY SINGLE thing created in AWS
  * key(project) -> value(project name)

## Amplify

## S3

1. Naming conventions
   1. [project] -> bucket for serving the production website
   2. [project]-test -> bucket for serving the production website to perform e2e tests on
   3. [project]-test-errors -> bucket for containing any info/ screenshots about errors when e2e testing the s3-test bucket

## DynamoDB

*

## CodeBuild

## API Gateway

* APT-Podcast-Studios
  * queries data from the Megaphone API about the podcasts in our network
  * receives a query and passes it on with authentication if the origin domain is in the allowed list in a lambda function and dynamically sets CORS headers for that origin

* APT-Worldwide
  * queries our Notes/ Domino server for information about worldwide

## Route 53

## Lambda functions

1. allowPodcastsTestOrigin -> dynamically sets `Access-Control-Allow-Headers:` to allow CORS for the prod or test s3 bucket for apt-podcasts
2. 

