pipeline {

    agent any

    stages{

        stage('clone the code') {

            steps {

                git 'https://github.com/sskamal88/mavenproject'

                sh 'mvn clean package'

            }
       }

	stage('deploy') {
		steps {
		sh 'cp target/JenkinsWar.war /var/lib/tomcat9/webapps/'		
		}
	}

    }

}

