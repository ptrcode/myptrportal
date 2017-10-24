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
        jiraGetIssueTransitions '$JIRA_ISSUE_KEY'
      }
    }
  }
}