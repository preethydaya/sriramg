pipeline {
    agent any

    stages {
        stage('one') {
            steps {
                echo 'project 1'
            }
        }
        stage('two') {
            steps {
                echo 'project 2'
            }
        }
        stage('three') {
            steps {
                echo 'project 3'
            }
        }
        stage('four') {
            steps {
                echo 'project 4'
            }
        }
        stage('five') {
            steps {
                echo 'project 5'
            }
        }

    }
    post {
      always {
        emailext(
        to: 'sriramgokulanathan@gmail.com',
        subject: '$DEFAULT_SUBJECT',
        body: '$DEFAULT_CONTENT',
        attachLog: true,
        mimeType: 'text/html'
      )
   }
 
 }
}
