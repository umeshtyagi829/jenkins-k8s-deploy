pipeline {
  agent any 
    stages{
      stage('app1'){
       when{
        expression{
          true
          }
         }
        steps{
          sh "kubectl apply -f deploy.yml --kubeconfig /admin.conf"
          }
        }
      }
  post{
    success{
      echo "success done"
      }
    failure{
      echo "fail"
      }
    always{
      echo "always"   
  }
  }
 }
        
