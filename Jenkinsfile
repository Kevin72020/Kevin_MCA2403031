CODE_CHANGES = true
pipeline{
  agent any
  stages{
    steps("build"){
       when {
         expression {
           BRANCH_NAME == 'development' && CODE_CHANGES == true
         }
       }
      steps{
            echo 'building the application...'
        }
    }  
steps("test"){
   when {
         expression {
           BRANCH_NAME == 'development' 
         }
       }
        steps{
            echo 'testing the application...'
        }
    }  
steps("deploy"){
	step{
	echo"deploy the application..."
 		}
	}
  }
}
