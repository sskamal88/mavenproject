pipeline {

    agent any

    stages{

        stage('clone the code') {

            steps {

                git 'https://github.com/sskamal88/mavenproject'

                sh 'mvn clean package'

            }
       }
	
	stage('approval for deployment') {
		steps {
		input('Do you want to deploy the code')
		}	
	}
	stage('deploy') {
		steps {
		sh 'cp target/JenkinsWar.war /var/lib/tomcat9/webapps/'		
		}
	}

    }

}

