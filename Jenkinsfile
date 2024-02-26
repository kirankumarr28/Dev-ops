pipeline {
  agent {
    node {
      label 'tesWorkSpace'
    }

  }
  stages {
    stage('jenkinsfile') {
      parallel {
        stage('jenkinsfile') {
          agent any
          steps {
            sh '''#!/bin/bash

echo "Created Blue Ocean Pipeline Successfully"'''
          }
        }

        stage('test') {
          steps {
            sh '''#!/bin/bash

echo "Hello BO"'''
          }
        }

      }
    }

  }
}