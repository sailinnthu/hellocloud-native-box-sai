# hellocloud-native-box

#### Create /etc/vbox/networks.conf
```
sudo su
cd /etc
mkdir vbox
cd vbox
vi networks.conf
* 0.0.0.0/0 ::/0
:wq!
```

#### Up and Running vagrant box
```
git clone git@github.com:hellocloudio/hellocloud-native-box.git
cd hellocloud-native-box
mkdir .ssh
cd .ssh
ssh-keygen
/Users/sai/hellocloud-boxes/hellocloud-native-box/.ssh/id_rsa
cd ../
vagrant up
```

#### Spin up k8s cluster
```
vagrant ssh
cd k8s-cop/1-single-cluster/setup/
./setup-kindcluster123.sh
```
