Vagrant.configure("2") do |config|

  config.vm.box = "ubuntu/focal64"

  # Configuração da placa de rede física em bridge com IP estático
  config.vm.network "public_network", ip: "172.16.17.120", bridge: "Realtek PCIe GbE Family Controller"

  # Sincronizar uma pasta para a Maquina Virtual (Por exemplo: um site, aplicação...)
  config.vm.synced_folder "../site", "/var/www/html"

  # Local onde posso customizar a maquina virtual
  config.vm.provider "virtualbox" do |vb|
    vb.gui = true #alterado de TRUE para FALSE para não abrir nenhuma interface gráfica.
    vb.name = "Site_H2TI"
    vb.cpus = "4"
    vb.memory = "4096" # alterndo memoria RAM de 1024 para 4096
  end

  # parte do PROVISION (Comandos pós criação).
  config.vm.provision "shell", inline: <<-SHELL
     apt-get update
     apt-get install -y apache2
    #  apt install -y nginx
   SHELL
end