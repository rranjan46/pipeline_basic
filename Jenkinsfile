pipeline {
agent any
stages {
stage("clone repo and clean it") {
steps {

sh "git clone https://github.com/rranjan46/pipeline_basic.git"
sh "mvn clean -f pipeline_basic"
}
}
stage("Test"){
steps {
sh "mvn test -f pipeline_basic"
}
}
stage("Deploy") {
steps {
sh "mvn package -f pipeline_basic"
}
}
}
}
