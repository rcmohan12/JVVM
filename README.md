# JVVM
Use Visual VM to connect to and monitior the memory usage of an application deployed on a remote host

## Download Links
- https://visualvm.github.io/download.html

## Environment details
- Windows 10 PC running the JVisualVM client
- RHEL host where the application is hosted on Glassfish5 app server

## Steps

1. Launch JVisual VM from your Windows machine. If there are any existing Java processes running on your system then, JVVM will display all of them under 'Local'.
2. To connect to a remote host, right click on 'Remote' --> Add Remote Host. Enter the host name and submit. 
3. To check if JVVM is able to connect to the host correctly, right click on the name and view its Properties. If you are able to view the DNS & IP of the host it indicates a successful connection.
5. In order to monitor Glassfish process on the remote host (where the application is deployed) , the JMX connection has to be enabled.

<img src ="images/dasboard.png"></img>
