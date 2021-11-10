pipeline {
    agent any 
    stages {
        stage('Linting') {
            steps {
                echo 'Linting ...'
                sh 'echo "Linting step" >> ./pipelinedemo1_shell_output.txt'
                sh 'date >> ./pipelinedemo1_shell_output.txt'
                sh 'gcc -c -fsyntax-only ./uptime.c'
            }
        }
        stage('Compiling') {
            steps {
                echo 'Compiling ...'
                sh 'echo "Compiling step" >> ./pipelinedemo1_shell_output.txt'
                sh 'date >> ./pipelinedemo1_shell_output.txt'
                sh 'gcc ./uptime.c'
            }
        }
    }
}
