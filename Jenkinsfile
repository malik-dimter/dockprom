node {
  stage('checkout scm') {
    checkout scm
  }

  stage('run grafana') {
    sh script: "docker-compose up -d", label: "starting App for production..."
    echo 'grafana: http://mmpro.frolleagues-dev.admiralcloud.com:3030'
    echo 'App is up and running ...'
  }
}