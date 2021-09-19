pipeline {
    agent any
      stages {
          stage('k8s_testing'){ 
              
                steps { 
                   
                    sh 'sudo kubectl get pod -o wide'
                    
                }
        }
         stage('gettingpod'){  
            
               steps {
                      sh 'sudo kubectl get pod -o wide '
                      sh 'sudo kubectl get svc'
             }
        }
    }
}
