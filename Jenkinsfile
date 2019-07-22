pipeline {
    agent any
	stages {
	    stages {'Clone Repo'} {
		    steps{
			sh"export AWS_DEFAULT_REGION=us-east-1"
			sh"aws cloudformation create-stack --stack-name group12 --template-body file://S3bucket.json --region 'us-east-1'"
			
			}
		}
	}	
}
