@Library('My-shared-library') _

pipeline{

  agent any

  stages{

    stage('git checkout'){

      steps{
          
          script{
            gitCheckout(
              branch: "main"
              url: "https://github.com/DeebakM/javaapp.git"
            )
          }
        
       
        
      }
    }
  }
}