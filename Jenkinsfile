CODE_CHANGES = getGitCHANGES()
pipeline {
    agent any

    stages {
        stage('Build') {
          when {
            expression {
                BRANCH_NAME == 'master' && CODE_CHANGES == true
            }
          }
            steps {
                echo 'Building the master branch..'
            }
        }
        stage('Test') {
          when {
            expression {
                BRANCH_NAME == 'master'
            }
          }
            steps {
                echo 'Testing the master branch..'
            }
        }
        stage('Deploy') {
          when {
            expression {
                BRANCH_NAME == 'master'
            }
          }
            steps {
                echo 'Deploying the master branch....'
            }
        }
    }
}
