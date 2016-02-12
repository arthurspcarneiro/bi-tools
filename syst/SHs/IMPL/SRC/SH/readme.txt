#colocar na pasta /usr/local/bin
#ao botar o sh em um ambiente, fazer na primeira vez
chmod 777 nome_arquivo
sed -i 's/\r$//' nome_arquivo 

#create_core
#Restart jboss: 
create_core -r nome_core
#Cria pastas do core
create_core nome_core

#drop_core
#Apaga tudo, e restart no jboss

#load_core
#carrega arquivo na pasta (nome_core)_dados
load_core nome_core arquivo

#truncate_core
#limpar o core, mas nao apaga os arquivos das pastas do core
truncate_core nome_core