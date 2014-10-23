lazys.sh
========

Lazy management of ssh and scp

This tool helps you to easily connect to all your servers and also to move files between your local computer and your servers.

The simple bash script lazys.sh does all the work for this.

If you simply call the script, it will list all the names of your connections. Simply type a name, hit enter and you will connect to your server.

To add a server to the list, run lazys.sh create $key $name@$server [$port]. $key is the key which you type to connect, $name is the user name, $server the domain name / IP address. The $port is optional, if you omit it, it defaults to 22.

To copy files instead of connecting to a server, you use the following commands:

lazys.sh cp $filePathOnServer $localFilePath -> Use scp to copy $filePathOnServer to $localFilePath

lazys.sh cpto $localFilePath $filePathOnServer -> Use scp to copy $localFilePath to $filePathOnServer

Enjoy and if you have any improvements, please send pull requests.
