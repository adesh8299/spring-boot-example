pipeline{
  agent any
  stages {
  stage('test') {
    steps {
      withMaven(globalMavenSettingsConfig: 'null', jdk: 'java', maven: 'maven', mavenSettingsConfig: 'null') {
      sh 'mvn clean install -s mvn-settings.xml'
}
    }
  }

  stage('package') {
    steps {
       withMaven(globalMavenSettingsConfig: 'null', jdk: 'java', maven: 'maven', mavenSettingsConfig: 'null') {
       sh 'mvn clean package'
    }
  }

}
  }
}
