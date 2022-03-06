pipeline {
    agent any

    stages {
        stage('1-build') {
            steps {
                echo 'build package'
            }
        }
         stage('2-test') {
            steps {
                echo 'test package'
            }
        }
         stage('3-deploy') {
            steps {
                echo 'Deploy package'
            }
        }
    }
    
    post {
        always {
            echo "pipeline completed"
            emailext body: 'Jenkins pipeline completed', subject: 'test', to: '9123086@gmail.com'
        }
    }
}
