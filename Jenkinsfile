pipeline {
  agent any

  environment{
    DIRECTORY_PATH = "/blob/main/Jenkinsfile"
    TESTING_ENVIRONMENT = "test-env"
    PRODUCTION_ENVIRONMENT = "LAKSHAY_LALIA"  
  }
  stages{
    stage('Build'){
      steps{ 
        echo "Fetch the source code from ${env.DIRECTORY_PATH}"
        echo "Compile the code and generate any necessary artifacts"
      }
    }
    stage('Test'){
      steps{
        echo "Unit tests"
        echo "Integration tests"
      }  
    }
    stage('Code Quality Check'){
      steps{
        echo "Check the quality of code"
      }  
    }
    stage('Deploy'){
      steps{
        echo "Deploy the application to a testing environment ${env.TESTING_ENVIRONMENT}"
      }  
    }
    stage('Approval'){
      steps{
     //  sh 'sleep(10)'
        echo "test"
      }  
    }
    stage('Deploy to Production'){
      steps{
        echo "Deploying the code to Production Environment ${env.PRODUCTION_ENVIRONMENT}"
      }  
    }
  }
}
