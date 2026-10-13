pipeline{
    agent any
    stages{
        stage("Restore dependences"){
            steps{
                bat "npm install"
            }
        }
        stage("Build application"){
            steps{
                bat "npm build --no-restore"
            }
        }
        stage("Run tests"){
            steps{
                bat "npm run test --no-build --verbosity normal"
            }
        }
    }
}