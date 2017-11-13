pipeline {
  agent any
  stages {
    stage('Build Pipeline') {
      parallel {
        stage('Build Pipeline') {
          steps {
            sleep 10
          }
        }
        stage('Code build') {
          steps {
            sh '''date 
echo "Code being simulate for flawless attributes"'''
            sleep 20
          }
        }
        stage('Code test') {
          steps {
            echo 'Build being to trigger the code test'
          }
        }
        stage('Code deploy') {
          steps {
            sleep 20
          }
        }
      }
    }
    stage('Deploy Pipeline') {
      parallel {
        stage('Deploy Pipeline') {
          steps {
            sleep 15
          }
        }
        stage('Deploy build') {
          steps {
            sh '''date 
 echo "Deploy code triggered to build"'''
            sleep 30
          }
        }
        stage('Deploy test') {
          steps {
            echo 'Deploy code begin to testing '
          }
        }
        stage('Trigger build') {
          steps {
            sleep 30
          }
        }
        stage('Trigger integrate testing') {
          steps {
            echo 'Integrating testing has completed successfully '
          }
        }
        stage('Trigger Auto Testing') {
          steps {
            sh '''date
 echo "Auto testing completed successfully"'''
            sleep 30
          }
        }
        stage('Deploy Code') {
          steps {
            sleep 25
          }
        }
      }
    }
    stage('Test Pipeline') {
      parallel {
        stage('Test Pipeline') {
          steps {
            sleep 15
          }
        }
        stage('Alpha Test') {
          steps {
            sleep 30
          }
        }
        stage('Beta Test') {
          steps {
            sleep 25
          }
        }
        stage('Destructive Test') {
          steps {
            echo 'Code being for destructive testing'
          }
        }
        stage('Continuous Test') {
          steps {
            echo 'Code being a continuous testing'
          }
        }
        stage('Functional Test') {
          steps {
            sh '''date 
echo "Code being to trigger functional testing"'''
          }
        }
        stage('Non-functional Test') {
          steps {
            sh '''date 
echo "Code being to trigger non functional testing"'''
          }
        }
        stage('Development Test') {
          steps {
            sleep 45
          }
        }
      }
    }
  }
}