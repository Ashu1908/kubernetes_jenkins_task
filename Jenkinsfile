pipeline {
    agent none
      stages {
          stage('k8s_testing'){  
               steps { 
                  sh 'sudo kubectl get pod -o wide'
             }
       }  
         
    }
}
