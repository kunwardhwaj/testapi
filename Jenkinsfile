
pipeline {

    agent any

    stages {

        stage('Deploy API to API manager') { // for display purposes

            steps {
                    bat "/var/lib/jenkins/swagger-promote-1.6.5/scripts/api-import.sh -c minimal-config-api-definition.json -s dev"

            }
        }

    }
    post {
        cleanup {
            deleteDir()
        }
    }
}
