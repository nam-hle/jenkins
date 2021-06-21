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
            perfReport compareBuildPrevious: true, filterRegex: '', modeEvaluation: true, modeOfThreshold: true, relativeFailedThresholdNegative: 0.0, relativeFailedThresholdPositive: -70.0, relativeUnstableThresholdNegative: 0.0, relativeUnstableThresholdPositive: -30.0, sourceDataFiles: 'TEST.xml'
        }
    }
}
