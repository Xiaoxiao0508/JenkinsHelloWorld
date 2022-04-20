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
          stage('Parallel') { 
            steps {
                parallel(
                    a:{echo "step a"
                      },
                    b:{echo "step b"
                      },
                     c:{echo "step c"
                      }
            }
        }
        
    }
}
