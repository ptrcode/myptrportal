pipeline {
  agent none
  stages {
    stage('verify') {
      steps {
        echo 'verified resource'
      }
    }
    stage('updateJira') {
      steps {
        jiraGetIssueTransitions(idOrKey: '$JIRA_ISSUE_KEY', site: 'http://10.10.10.50:8080/')
      }
    }
  }
}