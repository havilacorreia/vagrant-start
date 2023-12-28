# vagrant-start
 Conteúdo Incial sobre Vagrant

 ## Criar infraestrutura virtuais através de IaC - Infraestrutura como código

 O **Vagrant** só é possivel instalar na maquina física.

 VagrantFile (Customizações)

 * Sistema Operacional
 * Memória
 * CPU
 * Disco
 * Rede
 * Sincronizar uma pasta
 * Nome da Maquina
 * Provision (Script, Ansible, Puppet).

## Comandos na maquina física

 * vagrant init ubuntu/focal64 (Gera um arquivo VagrantFile)
 * vagrant up (Lê o arquivo e executa os comandos)
 * vagrant ssh (para acessar a Maquina Virtual)
 * vagrant reload (ler novamente o arquivo Vagrantfile e vai replicar as alterações)
 * vagrant destroy