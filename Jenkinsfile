pipeline {
  
  agent any
  
  parameters {
    choice (name: 'VERSION' , choices :['1','2','3'], description: 'Checking the parameters)
  
  stages{
    
    stage("Build") {
      when {
        expression{
          env.BRANCH_NAME =='dev'
        }
      }
          
      steps{
        echo 'Building process...Test2'
      }
    }
  
    stage("Test") {
      steps{
        echo 'Testing process...Test2'
        echo "deploying version : ${params.VERSION} "
      }
    }
    
    stage("Deploy") {

      steps{
        echo 'Deploying process...Test2'
      }
    }
  }
}

    
