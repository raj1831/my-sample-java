node
{
	stage('SCM Checkout')
	{
	git credentialsId: 'ccca2dd6-0b71-4dc4-8296-fac98a9c195e', url: 'https://github.com/raj1831/my-sample-java'
	}
	stage('Compile package')
	{
	sh label: 'Build package', script: 'mvn clean package'
	}
	stage('Build Image in docker')
	{
	sh label: 'Build Image', script: 'docker build -t raj1831/my-sample-java:1.0.0 .'
	}
}
