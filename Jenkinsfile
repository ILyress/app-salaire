node{
 stage('Clone') {
   git 'https://github.com/ILyress/app-salaire.git'
 }
 stage('Ansible') {
    ansiblePlaybook (
    colorized: true, 
    become: true, 
    playbook: 'install_table.yaml',
    inventory: 'inventaire.yaml',
    credentialsId: 'bd685dc9-3d1e-47b1-dfe5-49831f23062',
    disableHostKeyChecking: true
    )
  }
}
