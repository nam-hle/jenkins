pipeline {
    agent none
    stages {
        stage('Build') {
            stage('Build') {
                steps {
                    echo "Do Build"
                }
            }
        }
    }
    post {
        always {
            perfReport 'TEST-tree-engine.xml'
        }
    }
}
