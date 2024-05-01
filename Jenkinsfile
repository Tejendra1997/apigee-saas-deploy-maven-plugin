pipeline {
  agent any 
  tools {
    maven "maven-3.9.6"
  }
  stages {
    stage("Build_And_Deploy") {
      steps {
        script {
          echo "pwd $(pwd)"
          cd ./samples/forecastweatherapi-recommended/src/gateway/forecastweatherapi/
          echo "pwd $(pwd)"

          mvn --version
        }
      }
    }
  }
  post {
    always {
      echo "Devuda pipeline job success iyetatlu chai swaamy"
    }
    success {
      echo "Devudu karunichaadu"
    }
    failure {
      echo "Devudiki manasu ledu..."
    }
  }
}
