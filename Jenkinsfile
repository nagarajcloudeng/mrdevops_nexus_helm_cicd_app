pipline {
     agent any 
     stages {
       stage ('sonar code qualatiy'){
         agent {
            docker {
                image 'maven'

            }
         }
          steps {
              script{  
                   withSonarQubeEnv(credentialsId: 'sonar2') {
                
                   }
                   sh 'mvn clean package sonar:sonar'

              }
          }

            }
         }
          
         }
