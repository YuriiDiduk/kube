pipeline {
  agent any
     stages{
        stage('Deploy'){
 
            steps{
               sh 'kubectl apply -f k8s-spring-boot-deployment.yml'
              } 
            }
        stage('Deployc2'){
 
            steps{
               kubernetesDeploy configs: '', kubeConfig: [path: ''], kubeconfigId: 'config', secretName: '', ssh: [sshCredentialsId: '*', sshServer: ''], textCredentials: [certificateAuthorityData: '', clientCertificateData: '', clientKeyData: '', serverUrl: 'https://']
              } 
            }
        }
    }
