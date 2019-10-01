pipeline {
  agent any
  stages {
    stage('Weather check') {
      steps {
        sh '''#!/bin/bash
virtualenv venv --distribute
. venv/bin/activate 
pip install pytest pytest-cov
python WeatherReport.py < test_input.txt'''
      }
    }
  }
}