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
      stage('mvn test') {
          steps {
              script{
                sh 'mvn test'
              }
          }
      }
  }
}