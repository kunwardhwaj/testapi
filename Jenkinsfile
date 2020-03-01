
pipeline {

    agent any

    stages {

        stage('Deploy API to API manager') { // for display purposes

            steps {
                    bat "C:/Axway-7.6.2/Tools/apimanager-swagger-promote-1.6.5/swagger-promote-1.6.5/scripts/api-import.bat -c config/minimal-config-api-definition.json -s dev"

            }
        }

    }
    post {
        cleanup {
            deleteDir()
        }
    }
}
