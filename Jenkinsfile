node{
  def remote = [:]
  remote.name = 'oraclevm'
  remote.host = '152.67.160.182'
  remote.user = 'opc'
  remote.password = 'Muzammil073#'
  remote.allowAnyHosts = true
    stage('checkout') {
           checkout scm
  }  
  stage('Remote SSH') {
   // writeFile file: 'shaikimran07.sh', text: 'ls -lrt'
       // sshScript remote: remote, script: "shaikimran07.sh"
    sshCommand remote : remote, command: "pwd"
      sshCommand remote : remote, command: "cd /home"
    sshCommand remote : remote, command: "pwd"
      sshCommand remote : remote, command: "ls -lrt"
  }     
  stage('Remote SSH 2') {
    sshCommand remote : remote, command: "cd /home/opc/"
    sshCommand remote : remote, command: "mkdir shaikimran07.sh"
  }
}
