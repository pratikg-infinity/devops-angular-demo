pipeline{
    agent any
    stages{
        stage("build"){
            steps{
                echo "========executing build========"
                sh 'npm install'
                sh 'npm run build'   
            }
        }
        stage("test"){
            steps{
                echo "========executing test========"
                sh 'npm run test'
            }
        }
        stage("package"){
            steps{
                echo "========executing package========"                
            }
        }
        stage("publish"){
            steps{
                echo "========executing publish========"                            
            }
        }
        stage("deploy"){
            steps{
                echo "========executing deploy========"
            }
        }
    }
    post{
        always{
            echo "========always========"
        }
        success{
            echo "========pipeline executed successfully ========"
        }
        failure{
            echo "========pipeline execution failed========"
        }
    }
}