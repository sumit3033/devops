pipeline { 
agent any 
    stages { 
        stage ('Build') { 
            steps{
               echo "In Build Stage"
          }
        }
        stage ('Test') { 
           steps{
              sh "python3 test.py"
          }
        }
        stage ('QA') { 
           steps{ 
            echo "in QA Stage"
          }
        }
        stage ('Deploy') { 
           steps{
              sh "ansible-playbook network.yaml"
          }
        }
        stage ('Monitor') { 
           steps{
             echo "in Test stage"
           }
        }
    }           
 }
