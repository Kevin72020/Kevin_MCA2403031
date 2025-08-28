CODE_CHANGES = true
pipeline{
  agent any
  stages{
    stage("build"){
       when {
         expression {
           BRANCH_NAME == 'development' && CODE_CHANGES == true
         }
       }
      steps{
            echo 'building the application...'
        }
    }  
stage("test"){
   when {
         expression {
           BRANCH_NAME == 'development' 
         }
       }
        steps{
            echo 'testing the application...'
        }
    }  
stage("deploy"){
	step{
	echo"deploy the application..."
 		}
	}
  }
}
