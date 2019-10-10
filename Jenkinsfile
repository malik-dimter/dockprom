node {
  stage('checkout scm') {
    checkout scm
  }

  stage('run grafana') {
    sh script: "docker-compose -f docker-compose.yml -f docker-compose.prod.yml up -d", label: "starting App for production..."
    echo 'grafana: http://mmpro.frolleagues-dev.admiralcloud.com:3030'
    echo 'App is up and running ...'
  }
}