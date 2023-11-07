## Используя команду cat в терминале операционной системы Linux, создать два файла Домашние животные (заполнив файл собаками, кошками, хомяками) и Вьючные животными заполнив файл Лошадьми, верблюдами и ослы), а затем объединить их. Просмотреть содержимое созданного файла. Переименовать файл, дав ему новое имя (Друзья человека).
mkdir Kennel    
cd ~/Kennel    
cat > home_animals    
cat > pack_animals    
cat home_animals pack_animals > animals    
cat animals    
mv animals mans_friends    
ls -ali    

## Создать директорию, переместить файл туда.
cd ..    
mkdir Kennel_system    
cd ~/Kennel    
mv mans_friends ~/Kennel_system    
cd ~/Kennel_system    
ls -ali    

## Подключить дополнительный репозиторий MySQL. Установить любой пакет из этого репозитория.
sudo wget https://dev.mysql.com/get/mysql-apt-config_0.8.23-1_all.deb    
sudo dpkg -i mysql-apt-config_0.8.23-1_all.deb    
sudo apt-get update    
sudo apt-get install mysql-server    

## Установить и удалить deb-пакет с помощью dpkg.
sudo wget https://download.docker.com/linux/ubuntu/dists/jammy/pool/stable/amd64/docker-ce-cli_20.10.13~3-0~ubuntu-jammy_amd64.deb    
sudo dpkg -i docker-ce-cli_20.10.13~3-0~ubuntu-jammy_amd64.deb    
sudo dpkg -r docker-ce-cli    
