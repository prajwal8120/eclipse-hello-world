node{
    stage("src checkout") {
        git 'https://github.com/prajwal8120/eclipse-hello-world-.jar.git'
    }
    stage("Build Package") {
        sh "mvn clean package"
    }
    stage("Docker Build") {
        sh "docker build -f Dockerfile -t hello-world:1.0"
    }
}
