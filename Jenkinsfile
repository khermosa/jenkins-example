pipeline {
    agent any

    stages {
        stage ('Compile Stage') {

            steps {
                maven{
                    sh 'mvn clean compile'
                }
            }
        }

        stage ('Testing Stage') {

            steps {
                maven{
                    sh 'mvn test'
                }
            }
        }


        stage ('Deployment Stage') {
            steps {
                maven{
                    sh 'mvn deploy'
                }
            }
        }
    }
}
