pipeline {
    agent any
      stages {
         stage('k8s_testing'){  
               steps { 
                     sh 'sudo kubectl create deployment myd1 --image=ashut1908/k8s:v4'
                     sh 'sudo kubectl expose deploy myd1 --type=NodePort --port=80'
                    // sh 'sudo kubectl set image deployment myd1 k8s=ashut1908/k8s:v3'
                    // sh 'sudo kubectl get svc -o wide'
               } 
       }  
    }
} 
