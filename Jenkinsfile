pipeline {
    agent any

    stages {
        stage('1-build') {
            steps {
                echo 'build package add'
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
        stage('4-deploy2') {
            steps {
                echo 'Deploy2 package'
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
