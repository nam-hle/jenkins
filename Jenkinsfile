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
            perfReport compareBuildPrevious: true, modeOfThreshold: true, persistConstraintLog: true, relativeFailedThresholdPositive: 70.0, relativeUnstableThresholdNegative: -50.0, relativeUnstableThresholdPositive: 40.0, sourceDataFiles: 'TEST.xml'
        }
    }
}
