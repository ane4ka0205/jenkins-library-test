@Library('CommonLib@master') _

node {

  stage('poll the data') {
    git credentialsId: 'git_account', url: 'https://github.com/ane4ka0205/jenkins-global-lib.git'
  }

  stage('hello world') {
    job.hello()
  }

  stage('check the result') {
    json.showUserInfo("${workspace}/data.json")
  }


}
