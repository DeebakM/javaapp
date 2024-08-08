@Library('My_shared-library') _ 

pipeline{

  agent any

  stages{

    stage{

      steps('Git Checkout'){
                
          gitCheckout(
            branch: "main",
            url: "https://github.com/DeebakM/javaapp.git"
          )

      }
    }
  }
}