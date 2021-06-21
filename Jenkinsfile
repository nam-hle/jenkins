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
            perfReport compareBuildPrevious: true, filterRegex: '', modeOfThreshold: true, persistConstraintLog: true, relativeFailedThresholdNegative: 0.0, relativeFailedThresholdPositive: 80.0, relativeUnstableThresholdNegative: -50.0, relativeUnstableThresholdPositive: 50.0, showTrendGraphs: true, sourceDataFiles: 'TEST.xml'
        }
    }
}
