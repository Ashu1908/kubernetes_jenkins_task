pipeline {
    agent any
      stages {
          stage('k8s_testing'){  
               steps { 
                 // sh 'sudo kubectl get pod -o wide'
                  sh 'sudo docker ps'
               }
       }  
          
         stage('git'){  
            
               steps {
                      git branch: 'main', url: 'https://github.com/Ashu1908/kubernetes_jenkins_task.git'
               }
}

    }
}
