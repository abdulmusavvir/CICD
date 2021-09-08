pipeline{
 agent any
 stages{
    stage('common'){
      steps{
      echo 'common for all'
      }
    }
    stage('build for master'){
       when{
            expression{
                BRANCH_NAME == 'master'
            }
            } 
       steps{
            echo ' Build for master'
            }
    }
    stage('build for dev'){
       when{
            expression{
                BRANCH_NAME == 'dev'
            }
            } 
       steps{
            echo ' Build for dev'
            }
    }
    stage('build for feature'){
       when{
            expression{
                BRANCH_NAME == 'feature'
            }
            } 
       steps{
            echo ' Build for feature'
            }
    }
   }
  }
