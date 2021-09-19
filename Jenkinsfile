pipeline {
    agent any
      stages {
          stage('k8s_testing'){  
               
                steps { 
                   
                    sh 'sudo kubectl get pod -o wide'
                    
                }
        }  
         stage('gettingpod'){  
            agent {
                label 'master'
            } 
               steps {
                      sh 'sudo docker ps'
             }
        }
    }
}
