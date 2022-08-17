pipeline {
    agent any
    stages {
        stage("Test") {
            when {
                branch 'devel'
            }
            steps {
                def image_version = "${buildNumber}-${env.BRANCH_NAME}"
                echo 'image_version: ' + image_version
            }
        }
    }
}
