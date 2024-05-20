
Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/xenial64"

  
  config.vm.provision "shell", inline: <<-SHELL 
    echo "INSERT INTO gestion_restaurante.menu (nombre, descripcion, precio, categoria) VALUES " >> /home/vagrant/datos_menu.sql 
    echo "('Patatas 3 salsas', 'Si no te gusta la cabrales eres mala persona', 5, 'Entrante'), " >> /home/vagrant/datos_menu.sql 
    echo "('Kebab', 'Un kebap, mu rico mu bueno', 5, 'Entrante'), " >> /home/vagrant/datos_menu.sql 
    echo "('Frisuelos', 'NO, NO SON TORTITAS, FORIATON', 7.99, 'Postre');" >> /home/vagrant/datos_menu.sql 
  SHELL

end

