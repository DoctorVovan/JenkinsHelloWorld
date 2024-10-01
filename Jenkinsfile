pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello from jenkins file'
            }
        }
        stage('for the fix branch') {
            when {
                branch "fix*"
            }
            steps {
            echo 'this is only for fix'
               
            }
        }
        stage('for the PR') {
            when {
                branch 'PR-*'
            }
            steps {
                echo 'this only runs for the PRs testttt'
            }
        }
    }
}
