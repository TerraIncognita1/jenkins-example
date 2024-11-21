pipeline {
    agent any

    stages {
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean package' 
            }
        }

        stage ('Testing') {
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
