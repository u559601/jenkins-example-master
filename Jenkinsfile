pipeline {
    agent any
        tools {
            maven 'Apache Maven 3.5.2'
            jdk 'jdk1.8.0_121'
        }

    stages {
        stage ('Compile Stage') {

            steps {
                    sh 'mvn clean compile'
                }
            }


        stage ('Testing Stage') {

            steps {
                    sh 'mvn test'
                }
            }



        stage ('Deployment Stage') {
            steps {
                    sh 'mvn deploy'
                }
            }

    }
}