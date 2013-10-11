Install and configure Vagrant 
<code>
sudo apt-get install vagrant
</code>

Clone this repo
<code>
git clone https://github.com/ericwhyne/XData_Ubuntu_Hadoop.git
</code>

Go to the repo directory and start the environment
<code>
cd ...
vagrant up
</code>

Wait for vagrant to configure the VM, then connect the host machine to the XData VPN.

Log in to the VM and switch to the hdfs user
<code>
vagrant ssh
su hdfs (password is xdata)
cd ~ 
</code>

Use scripts to view HDFS file system or run the hadoop streaming tests
From /home/hdfs/ as hdfs user run
<code>
./scripts/compute-hdfs -ls /
</code>
