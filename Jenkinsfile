pipeline {
	agent{
	label 'mens-label'
	}
	stages {
	    stage('Checkout') {
	        steps {
			checkout scm			       
		      }}
		stage('Build') {
	           steps {
			  sh '/home/grras/slave-dir/apache-maven-3.9.5/bin/mvn install'
	                 }}
		stage('Deployment'){
		    steps {
			sh 'cp target/grras6.war /home/grras/slave-dir/apache-tomcat-9.0.82/webapps'
			}}	
}}
