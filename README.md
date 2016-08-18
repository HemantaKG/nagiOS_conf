# nagiOS3 configuration

Follow below step to cofigure nagios3:

step 1. Nagios drops configuration files into /etc/nagios3/conf.d/ as part of the base installation, (use those bases and template files for configuration Nagios)

step 2. create a file named "cluster-nagios.cfg" under configuration folder "/etc/nagios3/conf.d/"

NOTE: This file keeps entire cluster asscess or comunication related informations of each node of the cluster to communicate with the nodes for monitoring the states

cd /etc/nagios3/conf.d/

nano cluster-nagios.cfg

step 3. Next, try to start up (or restart) nagios

NOTE: the basic setup done

Advance configuration to monitor LOAD, CPU, USERS, IPMI, ect...

NOTE: look at the "/etc/nagios3/conf.d/localhost_nagios2.cfg" file

Other:

1. to change nagios3 passwd (that we set at step 2)

sudo htpasswd -c /etc/nagios2/htpasswd.users nagiosadmin
