pipeline {

    agent any

    stages{

        stage('clone the code') {

            steps {

                git 'https://github.com/sskamal88/mavenproject'

                sh 'mvn clean package'

            }

       }

    }

}

