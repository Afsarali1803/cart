pipeline{
    agent any

    stages{
        stage(" Lint check"){
            steps{
                sh "npm i jslint"
                sh "~/node_module/jslint/bin/jslint.js server.js"
            }
            
        }

        stage(" Code Quality Checks"){
            steps{
                sh "echo Sonarcube"
                sh ""
            }
            
        }
    }
    
}