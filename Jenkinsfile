pipeline {
  agent none
  stages {
    stage('verify') {
      steps {
        echo 'verified resource'
        sh 'echo papu'
        echo 'ssss'
      }
    }
    stage('updateJira') {
      steps {
        jiraGetIssueTransitions(idOrKey: '$JIRA_ISSUE_KEY', site: 'myjira')
      }
    }
  }
}