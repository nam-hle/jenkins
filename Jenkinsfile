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
            perfReport sourceDataFiles: 'TEST.xml', compareBuildPrevious: true, excludeResponseTime: true, modePerformancePerTestCase: true, showTrendGraphs: true
        }
    }
}
