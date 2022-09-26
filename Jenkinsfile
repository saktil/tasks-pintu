node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'leon'){
        def customImage = docker.build("leonswww/node-app")
        customImage.push()
    }
}