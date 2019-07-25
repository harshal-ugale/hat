pipeline 
{
    agent any
	stages {
	    stage ('Clone Repo') {
		    steps {
			sh "export AWS_DEFAULT_REGION=us-east-1"
			sh "aws cloudformation create-stack --stack-name ${params.stackname} --template-body file://S3bucket.json --Parameters file://parameter.json  --region 'us-east-1'"
			
			} 
		}
	}	
}
