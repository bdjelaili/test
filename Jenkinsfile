docker.withServer('tcp://swarm.mycorp.com:2376', 'swarm-certs') {
  docker.image('httpd').withRun('-p 8080:80') {c ->
    sh "curl -i http://${hostIp(c)}:8080/"
  }
}
def hostIp(container) {
  sh "docker inspect -f {{.Node.Ip}} ${container.id} > hostIp"
  readFile('hostIp').trim()
}
