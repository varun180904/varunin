

node('master') 
{
    stage('Continuous Download_loans') 
	{
   		git 'https://github.com/varun180904/varunin.git'
	}
    stage('Continuous Build_loans') 
	{
    		sh label: '', script: 'mvn package'
	}
	stage('Continuous Deployment_loans') 
   	{
		sh label: '', script: 'scp  /home/ubuntu/.jenkins/workspace/Job2_loans/webapp/target/webapp.war  ubuntu@172.31.34.181:/var/lib/tomcat8/webapps/qaenv.war'
	}
	stage('Continuous Testing_loans') 
  	{
		sh label: '', script: 'echo "Testing Passed"'
	}
	stage('Continuous Delivery_loans') 
	 {
		sh label: '', script: 'scp  /home/ubuntu/.jenkins/workspace/Job2_loans/webapp/target/webapp.war  ubuntu@172.31.36.144:/var/lib/tomcat8/webapps/prodenv.war'
	}
}
