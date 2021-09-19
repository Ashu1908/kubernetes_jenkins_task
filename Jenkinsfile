pipeline {
    agent none
      stages {
         // stage('k8s_testing'){  
           //     steps { 
             //       sh 'sudo kubectl get pod -o wide'
             //  }
       // }  
         stage('gettingpod'){  
            agent {
                label 'master'
            } 
               steps {
                      //sh 'sudo /usr/bin/docker ps'
                       sh 'sudo mkdir /test123'
               }
        }
    }
}
