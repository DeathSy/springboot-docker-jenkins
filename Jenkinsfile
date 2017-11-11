node {
  stage 'Building image'
  git  ''
  def myEnv = docker.build 'cqueiroz:snapshot'
  myEnv.inside {
    sh 'mvn clean package'
  }
}