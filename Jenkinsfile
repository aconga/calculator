pipeline {
agent any
stages {
stage("Package") {
steps {
sh "./gradlew compileJava"
}
}
stage("Docker build") {
steps {
sh "docker build -t leszko/calculator ."
}
}
}
}