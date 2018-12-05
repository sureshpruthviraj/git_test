pipeline {
  agent none
  stages {
    stage('job1') {
      steps {
        sh 'python3 /home/suresh/jenkins/job_1.py'
      }
    }
    stage('job2') {
      parallel {
        stage('job2') {
          steps {
            sh 'python3 /home/suresh/jenkins/job_2.py'
          }
        }
        stage('job3') {
          steps {
            sh 'python3 /home/suresh/jenkins/job_3.py'
          }
        }
      }
    }
  }
}