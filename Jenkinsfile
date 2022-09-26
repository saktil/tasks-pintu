node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'dockerhub'){
        def customImage = docker.build("leonswww/node-app")
        customImage.push()
    }
}