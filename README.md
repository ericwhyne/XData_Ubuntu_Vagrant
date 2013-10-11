Install and configure Vagrant 
sudo apt-get install vagrant

Clone this repo
git clone https://github.com/ericwhyne/XData_Ubuntu_Hadoop.git

Go to the repo directory and start the environment
cd ...
vagrant up

Wait for vagrant to configure the VM, then connect the host machine to the XData VPN.

Log in to the VM and switch to the hdfs user
vagrant ssh
su hdfs (password is xdata)
cd ~ 

Use scripts to view HDFS file system or run the hadoop streaming tests
From /home/hdfs/ as hdfs user run
./scripts/compute-hdfs -ls /
