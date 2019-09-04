node {
	stage('SCM Checkout')
	{
	git 'https://github.com/raj1831/my-sample-java'
	}

	stage('Compile package')
	{
	sh label: 'Build', script: 'mvn package'
	sh lavel: 'Coping Artifacts', /bin/cp target/*.war docker/
	}

}
