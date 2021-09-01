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
}
