# JVVM
Use Visual VM to connect to and monitior the memory usage of an application deployed on a remote host

## Download Links
- https://visualvm.github.io/download.html

## Environment details
- Windows 10 PC running the JVisualVM client
- RHEL host where the application is hosted on Glassfish5 app server

## Steps

1. Launch JVisual VM from your Windows machine. If there are any existing Java processes running on your system then, JVVM will display all of them under 'Local'.

![alt text](https://github.com/rcmohan12/JVVM/blob/main/images/dashboard.png)

2. To connect to a remote host, right click on 'Remote' --> Add Remote Host. Enter the host name and submit. 
3. To check if JVVM is able to connect to the host correctly, right click on the name and view its Properties. If you are able to view the DNS & IP of the host it indicates a successful connection.
5. In order to monitor Glassfish process on the remote host (where the application is deployed) , the JMX connection has to be enabled. To do this, right click on the remote host configured in step 2 and select 'Add JMX Connection'. Here, enter the JMX port configured for the remote host. In this pre configured Glassfish server, the port number was taken from the domain.xml file. 
6. Once the JMX port is configured, connect to the remote host. If there is no firewall blocking the connection then, the Glassfish process with its associated PID will be displayed.
7. If there is firewall blocking the connection, then the process will not show up (yet to figure out how to work around the firewall)

