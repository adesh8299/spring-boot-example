pipeline{
  agent any
  stages {
  stage('test') {
    steps {
      withMaven(globalMavenSettingsConfig: 'null', jdk: 'java', maven: 'maven', mavenSettingsConfig: '8b4b7602-2943-4315-899a-b24e82e8f4c6') {
      sh 'mvn clean install -s mvn-settings.xml'
}
    }
  }

  stage('package') {
    steps {
       withMaven(globalMavenSettingsConfig: 'null', jdk: 'java', maven: 'maven', mavenSettingsConfig: '8b4b7602-2943-4315-899a-b24e82e8f4c6') {
       sh 'mvn clean package'
    }
  }

}
  }
}
