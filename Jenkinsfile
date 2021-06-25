pipeline {
  
  agent any
  
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
        echo env.BRANCH_NAME
      }
    }
    
    stage("Deploy") {
      when {
        expression{
          env.BRANCH_NAME =='main'
        }
      }
      steps{
        echo 'Deploying process...Test2'
      }
    }
  }
}

    
