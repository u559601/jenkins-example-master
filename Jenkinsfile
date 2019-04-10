pipeline {
    agent any
        tools {
            maven 'Apache Maven 3.5.2'
            jdk 'jdk1.8.0_121'
        }

    stages {
        stage ('Compile Stage') {

            steps {
                    bat 'mvn clean compile'
                }
            }


        stage ('Testing Stage') {

            steps {
                    bat 'mvn test'
                }
            }



        stage ('Deployment Stage') {
            steps {
                    bat 'mvn deploy'
                }
            }

    }
}