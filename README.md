# vagrant-start
 Conteúdo Incial sobre Vagrant

 Criar infraestrutura virtuais através de IaC - Infraestrutura como código

 O **Vagrant** só é possivel instalar na maquina fisica.

 VagrantFile
 - SO
 - Memória
 - CPU
 - Disco
 - Rede
 - Sincronizar uma pasta
 - Nome da Maquina
 - Provision (Script, Ansible, Puppet).


Comando na maquina física

 vagrant init ubuntu/focal64 (Gera um arquivo VagrantFile)
 vagrant up (Lê o arquivo e executa os comandos)
 vagrant ssh (para acessar a Maquina Virtual)
 vagrant destroy