@Library('roboshop-shared-library@main')
pipeline{
    agent any
    stages {
        stage ( " Lint check" ) {
            steps{
                scripts {
                    sample.info{'Training', 'facebook.com'}
                }
                sh "npm i jslint"
                sh "node_module/jslint/bin/jslint.js server.js || true"
                sh "echo Lint check completed"
            }    
        }
        stage ( " Code Quality Checks" ) {
            steps{
                sh "echo Sonarcube"
            }    
        }
    }
}