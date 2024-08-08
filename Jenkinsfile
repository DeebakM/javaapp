@Library('My-shared-library@main') _

pipeline {
  agent any

  stages {
      stage('git checkout') {
          steps {
              script{
                gitCheckout([
                  url: 'https://github.com/DeebakM/javaapp.git',
                  branch: 'main'
                ])
              }
          }
      }
      
      stage('maven test') {
        script {
          echo 'running test',
          sh 'mvn test'
        }

      }
  }
}