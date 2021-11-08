pipeline {
    agent any 
    stages {
        stage('Linting') {
            steps {
                echo 'Linting ...'
                sh 'date >> ./pipelinedemo1_shell_output.txt'
                sh 'gcc -c -fsyntax-only ./uptime.c'
            }
        }
        stage('Compiling') {
            steps {
                echo 'Compiling ...'
                sh 'date >> ./pipelinedemo1_shell_output.txt'
                sh 'gcc ./uptime.c'
            }
        }
    }
}
