pipeline {
    agent any
    stages {
        stage('Build') {
            
            steps {
                echo 'Build step'
                
            }
        }
        stage('Test') {
            
            steps {
                catchError(buildResult: 'SUCCESS', stageResult: 'FAILURE'){
                echo 'Test step'
                sh 'exit 1'
                }
            }
        }
        stage('Deploy') {
            
            steps {
                echo 'Deploy step'
                  }
            }
      }
}
