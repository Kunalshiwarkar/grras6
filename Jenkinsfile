pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo "Hello kunal"
          stage('Build') {
	           steps {
			  sh '/Documents/Devops_software/tar/apache-maven-3.9.5/bin/mvn install'
	                 }}
		stage('Deployment'){
		   steps {
		sh 'cp target/grras6.war /home/kunal/Documents/Devops_software/tar/apache-tomcat-9.0.82/webapps'
			}}      
            }
        }
    }
}
