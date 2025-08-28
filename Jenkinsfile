CODE_CHANGES = true
pipeline{
  agent any
  stages{
    step("build"){
       when {
         expression {
           BRANCH_NAME == 'development' && CODE_CHANGES == true
         }
       }
      steps{
            echo 'building the application...'
        }
    }  
step("test"){
   when {
         expression {
           BRANCH_NAME == 'development' 
         }
       }
        steps{
            echo 'testing the application...'
        }
    }  
step("deploy"){
	step{
	echo"deploy the application..."
 		}
	}
  }
}
