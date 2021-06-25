pipeline {
  
  agent any
  
  stages{
    
    stage("Build") {
      when {
        expression{
          BRANCH_NAME =='dev'
        }
      }
          
      steps{
        echo 'Building process...Test2'
      }
    }
  
    stage("Test") {
      steps{
        echo 'Testing process...Test2'
      }
    }
    
    stage("Deploy") {
      steps{
        echo 'Deploying process...Test2'
      }
    }
  }
}

    
