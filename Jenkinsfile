node('master') 
{
    stage('Continuous Download_master') 
    {
    	git 'https://github.com/varun180904/varunin.git'
    }

    stage('Continuous Build_master') 
	{
    sh label: '', script: 'mvn package'
	}
}
