pipeline {
  agent any
  stages {
    stage('Weather check') {
      steps {
        sh '''pip install pytest pytest-cov
python WeatherReport.py < test_input.txt'''
      }
    }
  }
}