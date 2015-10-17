# Dreamhost-Install-Custom-Python-Version-Django
Install Django and Custom Python Version in Dreamhost

Credit goes to Josh and his webpage:
http://www.mixtmeta.com/blog/python-on-dreamhost-part-1

//Install custom python version
ssh into your hosting root
wget https://www.python.org/ftp/python/3.5.0/Python-3.5.0.tgz --no-check-certificate
tar -xzvf Python-3.5.0.tgz
cd Python-3.5.0
./configure --prefix=$HOME/.python3.5.0
make
make install
cd $HOME/.python3.5.0/bin
./pip3.5 install virtualenv

//Install django
