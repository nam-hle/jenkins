pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo "Do Build"
            }
        }
    }
    post {
        always {
            perfReport 'TEST-tree-engine.xml'
        }
    }
}
