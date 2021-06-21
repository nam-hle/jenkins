pipeline {
    agent none
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
