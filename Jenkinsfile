pipeline {
  agent none
  stages {
    stage('mygroup') {
      parallel {
        stage('mygroup') {
          steps {
            echo 'verified resource'
            sh 'echo papu'
            echo 'ssss'
            echo 'ssss'
            sh 'ssss'
            bat 'ssss'
          }
        }
        stage('') {
          steps {
            echo 'assss'
            echo 'ssdsd'
            sleep 566
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