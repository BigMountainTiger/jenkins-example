pipeline {
    agent any

    stages {
        stage('Step_0') {
            steps {
                sh '''
                    echo "Starting the step 0"
                    pwd
                    A_VAR="This is the value of the variable"
                    echo "$A_VAR"
                    bash --version
                    java -version
                    cat /etc/os-release
                    ls -la
                '''
            }
        }
        stage('Step_1') {
            steps {
                sh 'echo "Starting the step 1"'
            }
        }
        stage('Step_2') {
            steps {
                sh 'ci/tasks/task_1'
            }
        }
    }
}
