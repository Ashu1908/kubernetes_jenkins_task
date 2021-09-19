pipeline {
    agent any
      stages {
           
          
         stage('git'){  
               steps {
                      git branch: 'main', url: 'https://github.com/Ashu1908/kubernetes_jenkins_task.git'
                      sh 'sudo cp -rvf * /test'
                      sh 'sudo docker build -t ashut1908/k8s:v1  /test'
                      sh 'sudo docker login -u ashut1908  -p Rahul@123'
                      sh 'sudo docker push ashut1908/k8s:v1'   
               }
}
         stage('k8s_testing'){  
               steps { 
                      sh 'sudo kubectl create deployment myd --image=ashut1908/k8s:v1'
                      sh 'sudo kubectl expose deploy myd --type=NodePort --port=80'
                      sh 'sudo kubectl get svc -o wide'
               }
       } 
    }
}
