node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'leon'){
        def customImage = docker.build("leonswww/node-app")
        customImage.push()
    }

    # deploy to kubernetes
    # kubernetesDeploy(configs: "deploymentservice.yml", kubeconfigId: "kubernetes")
}