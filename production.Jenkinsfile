pipeline {
    agent any
    // options {
    //     skipDefaultCheckout true
    // }
    stages {
        stage('list workspace files') {
            steps {
                sh('ls -lh')
            }
        }
        // stage('clean_workspace_and_checkout_source') {
        //     steps {
        //         sh('ls -lh')
        //         deleteDir()
        //         checkout scm
        //     }
        // }
        stage('check git file size') {
            steps {
                sh('du -sh .git')
            }
        }
        stage('build') {
            steps {
                echo 'i build therefore i am'
            }
        }
    }
}
