pipeline {
  agent any
  stages {
    stage('Weather check') {
      steps {
        sh '''pipeline {
    agent none 
    stages {
        stage(\'Build\') { 
            agent {
                docker {
                    image \'python:2-alpine\' 
                }
            }
            steps {
                sh \'python WeatherReport.py < test_input.txt\' 
            }
        }
    }
}'''
        }
      }
    }
  }