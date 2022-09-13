pipeline{
  agent any
  stages {
  stage('test') {
    steps {
      withMaven(gglobalMavenSettingsConfig: 'null', jdk: 'null', maven: 'maven', mavenSettingsConfig: 'null') {
      sh 'mvn clean test'
}
    }
  }

  stage('package') {
    steps {
       withMaven(globalMavenSettingsConfig: 'null', jdk: 'null', maven: 'maven', mavenSettingsConfig: 'null') {
       sh 'mvn clean package'
    }
  }

}
  }
}
