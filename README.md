# just_BI_api

# Installing
run:  
`npm i`
  
rename config.json.example to config.json:  
`cp config.json.example config.json`  
  
configure your config.json  
You're ready!
  
# Tests TDD
open your terminal on project repo and write  
for all tests `npm test`  
for one test `mocha -g "[test name]"`  
  
# Start server
open your terminal on project repo and write  
`npm start` or `node server.js`  
  
# awscli
configure awscli

    aws configure

list all buckets and objetcts

    aws s3 ls

list all buckets and objetcts in specific target

    aws s3 ls s3://awsnode.actualit.info/

Create bucket

    aws s3 mb s3://awsnode.actualit.info

Delete bucket (recursively)

    aws s3 rb s3://awsnode.actualit.info --force

Upload object

    aws s3 cp awstest.txt s3://awsnode.actualit.info/example/
    // to copy the file on example dir do not forget the /,  
    // without the / your copy'll be renamed from awstest.txt to example

Delete object

    aws s3 rm s3://awsnode.actualit.info/example/filename.txt

# Rekognition of faces

    aws rekognition detect-faces --image "S3Object={Bucket=awsnode1.actualit.info,Name=gandhi.png}" --region eu-west-1
    