# Disable transparent hugepages
Shell script init for THP disable

 move disable-transparent-hugepages to 

/etc/init.d/

make executable and change permission 
<pre><code>
sudo chmod 755 /etc/init.d/disable-transparent-hugepages
</code></pre>

Configure your operating system to run it on boot.

<h4> Distribution	Command </h4>
 Ubuntu and Debian 
<pre><code>
sudo update-rc.d disable-transparent-hugepages defaults
</code></pre>
SUSE
<pre><code>
sudo insserv /etc/init.d/disable-transparent-hugepages
</code></pre>
Red Hat, CentOS, Amazon Linux, and derivatives	
<pre><code>
sudo chkconfig --add disable-transparent-hugepages
</code></pre>
