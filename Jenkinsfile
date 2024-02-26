pipeline {
  agent {
    node {
      label 'tesWorkSpace'
    }

  }
  stages {
    stage('jenkinsfile') {
      parallel {
        stage('jenkinstestfile') {
          agent {
            node {
              label 'TestLable'
            }

          }
          environment {
            ubuntu = 'PuTTY-User-Key-File-2: ssh-ed25519 Encryption: none Comment: test_instance Public-Lines: 2 AAAAC3NzaC1lZDI1NTE5AAAAIDuYhkp96/eTpgGwhe86giebUUXl/pMnGrnBXp9d y0n4 Private-Lines: 1 AAAAIDBRAgEBMAUGAytlcAQiBCBLO2ZA3BkP1bGNI2D4WKwh Private-MAC: 5d9f22c9ad1e23ea687ea2fafd5f366b6bb7a9c9'
          }
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