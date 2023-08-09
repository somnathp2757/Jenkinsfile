pipeline{
    agent any
    
    stages{
        stage("Test"){
            steps{
                echo "mvn test"
            }

        }

        stage("Build"){
            steps{
                echo "Build"
            }

        }
    
        stage("stage"){
            steps{
                echo "Deploy to stage"
            }

        }
    
        stage("Production"){
            steps{
                echo "Deploy to production"
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
