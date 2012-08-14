#HostingScripts
These are basic scripts used to make hosting simpler on my CentOS setup

##enablewww
`enablewww username domainincluding.com`
 _enablewww_ enables hosting for the specified domain and username.
 If the user doesnt exist it will create it, so you probably have to run this as sudo.
 This creates a directory structure under /home/username/ and should set permissions properly.
 It also creates the vhosts file for apache and the configuration for named (the DNS service).
 THIS OVERWRITES CONFIGURATIONS for now

##enabledns
`enabledns username domaincluding.com`
 _enabledns_ enables domain name hosting on your self-hosted name server.

##disablewww
`disablewww username domainincluding.com`
 _disablewww_ disables the hosting for the specified domain under the user.
 This just destroys symlinks and no actual configurations.

##listww
`listwww`
 _listwww_ lists all the enabled sites on this server
 It's a nice way of seeing which vhosts are being used 

##hosting.conf
 _hosting.conf_ is a file that contains some configuration variables for the system
 Modify this to adjust these scripts for your system.
 An ubuntu setup is provided in hosting.ubuntu.conf. Overwrite hosting.conf with that for ubuntu.
last update: 08.14.2012
http://www.github.com/twohlix/
