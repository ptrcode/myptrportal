pipeline {
  agent none
  stages {
    stage('mygroup') {
      parallel {
        stage('Provision') {
          steps {
            echo 'verified resource'
            sh 'echo papu'
            echo 'ssss'
            echo 'ssss'
            sh 'ssss'
            bat 'ssss'
          }
        }
        stage('network') {
          steps {
            echo 'assss'
            echo 'ssdsd'
            sleep 566
          }
        }
        stage('') {
          agent any
          steps {
            echo 'sdddd'
          }
        }
      }
    }
    stage('updateJira') {
      steps {
        jiraGetIssueTransitions(idOrKey: '$JIRA_ISSUE_KEY', site: 'myjira')
      }
    }
  }
}