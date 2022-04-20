pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                echo "Build stage"
            }
        }
        stage('Test') { 
            steps {
                 echo "Test stage"
            }
        }
        stage('Deploy') { 
            steps {
                 echo "Deploy stage"
            }
        }
//          stage('Check') { 
//             steps {
//                  input("Do you want to check the resule?")
//             }
//         }
          stage('SendMail') { 
            steps {
                mail body:"$(env.JOB_NAME} - Build # ${env.BUILD_NUMBER}-${currentBuild.currentResult}",subject:"${env.JOB_NAME} - Build # ${env.BUILD_NUMBER}-${currentBuild.currentResult}",to:'cxxmelbourne@hotmail.com
            }
        }
        
    }
}
