Jenkinsfile
  pipeline {
    agent any
	 stages{
	  stage('build'){
	   steps {
	    sh 'mvn clean package'
		}
		post {
		success {
		
		echo 'Now archiving ...'
		archiveArtifacts atifacts:'**target/*.war'
        }
}
}
}
}
		