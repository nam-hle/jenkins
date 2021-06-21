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
            perfReport 'TEST.xml', compareBuildPrevious: true, excludeResponseTime: true, modePerformancePerTestCase: true, showTrendGraphs: true
        }
    }
}
