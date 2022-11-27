@Library('roboshop-shared-library@main') _

pipeline {
    agent any
    stages {
        stage ( " Lint check" ) {
            steps {
                script {
                    sample.info ()
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