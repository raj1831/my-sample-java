node
{
	stage('SCM Checkout')
	{
	git 'https://github.com/raj1831/my-sample-java'
	}

	stage('Compile package')
	{
	sh label: 'Build', script: 'mvn package'
	}

	stage('Copying Artifacts')
	{
	sh label: 'Copy', script: 'cp target/*.war Docker'
	}
}
