pipeline {
    agent any

    stages {
        stage ('Compile Stage') {

            steps {
                maven : 'maven_3_5_2' {
                    sh 'mvn clean compile'
                }
            }
        }

        stage ('Testing Stage') {

            steps {
                maven : 'maven_3_5_2' {
                    sh 'mvn test'
                }
            }
        }


        stage ('Deployment Stage') {
            steps {
                maven : 'maven_3_5_2' {
                    sh 'mvn deploy'
                }
            }
        }
    }
}
