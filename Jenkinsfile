node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'dockerhub'){
        def customImage = docker.build("saktil/nodeapp")
        customImage.push()
    }
    
    # deploy to kubernetes
   # kubernetesDeploy(configs: "deploymentservice.yml", kubeconfigId: "kubernetes")
}
Footer

