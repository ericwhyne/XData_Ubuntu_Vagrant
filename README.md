Install and configure Vagrant<br>
<code>sudo apt-get install vagrant</code>

(Optional) Add Vagrant plugin that keeps Virtual Box Guest Additions in sync.<br>
<code>vagrant plugin install vagrant-vbguest</code>

Clone this repo<br>
<code>git clone https://github.com/ericwhyne/XData_Ubuntu_Hadoop.git</code>

Go to the repo directory and start the environment<br>
<code>cd ..</code><br>
<code>vagrant up</code><br>

Wait for vagrant to configure the VM, then connect the host machine to the XData VPN.

Log in to the VM and switch to the hdfs user<br>
<code>vagrant ssh</code><br>
<code>su hdfs</code> (password is xdata)<br>
<code>cd ~ </code><br>

Use scripts to view HDFS file system or run the hadoop streaming tests.<br>
From /home/hdfs/ as hdfs user:<br>
<code>./scripts/compute-hdfs -ls /</code><br>


To have Vagrant sync the Guest Additions for Virtual Box do the following:
$ # For vagrant < 1.1.5:
$ # vagrant gem install vagrant-vbguest

$ # For vagrant 1.1.5+ (thanks Lars Haugseth):
$ vagrant plugin install vagrant-vbguest
