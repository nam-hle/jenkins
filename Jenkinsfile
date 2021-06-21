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
            perfReport compareBuildPrevious: true, modeOfThreshold: true, persistConstraintLog: true, relativeFailedThresholdPositive: 80.0, relativeUnstableThresholdNegative: -50.0, relativeUnstableThresholdPositive: 50.0, showTrendGraphs: true, sourceDataFiles: 'TEST.xml'
        }
    }
}
