pipeline {
  agent any
     stages{
        stage('Deploy'){
 
            steps{
               sh 'kubectl apply -f k8s-spring-boot-deployment.yml'
              } 
            }
        }
    }
