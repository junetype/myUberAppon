 36  wget -qO - https://www.mongodb.org/static/pgp/server-3.2.asc | sudo apt-key add -
   37  echo "deb http://repo.mongodb.org/apt/ubuntu xenial/mongodb-org/3.2 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-3.2.list
   38  sudo apt-get update
   39  sudo apt-get install -y mongodb-org
   40  service mongod restart
   41  curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.37.2/install.sh | bash
   42  source ~/.bashrc  && nvm install  v6.17.1 
#setup-------------------------------------------
