pipeline{
    agent any
    stages{
        stage("Restore dependences"){
            steps{
                bat "npm install"
            }
        }
        stage("Run tests"){
            steps{
                bat "npm run test"
            }
        }
    }
}