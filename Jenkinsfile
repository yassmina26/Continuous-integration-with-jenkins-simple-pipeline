Pipeline{
  agent any //execute on any node 
  stages{
    stage('fetch code'){
      steps{
        git branch: 'paac', url: 'https://github.com/devopshydclub/vprofile-project.git'
      }
    }
    stage('Build'){ //build stage
      steps{
        sh 'mvn install'
      }
    }
    stage('test'){
      steps{
        sh 'mvn test'
      }
    }
  }
} 