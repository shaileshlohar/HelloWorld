pipeline {
         agent any
         stages {
                 stage('Build') {
                 steps {
                     echo 'Hi, This is build stage.'
                 }
                 }
                 stage('Test') {
                 steps {
                    echo 'Hi, This is Test stage.'
                 }
                 }
                 stage('Deploy') {
                 parallel { 
                            stage('Deploy start ') {
                           steps {
                                echo "Start the deploy .."
                           } 
                           }
                            stage('Deploying now') {
                            
                              steps {
                                echo "Docker Created"
                              }
                           }
                           }
                           }
                 stage('Prod') {
                     steps {
                                echo "App is Prod Ready"
                              }
                 
              }
}
}
