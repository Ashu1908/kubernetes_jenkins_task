pipeline {
    agent any
      stages {
         stage('k8s_testing'){  
               steps { 
                      sh 'sudo kubectl create deployment myd1 --image=ashut1908/k8s:v1'
                      sh 'sudo kubectl expose deploy myd1 --type=NodePort --port=80'
                      sh 'sudo kubectl get svc -o wide'
               }
       }  
    }
}
