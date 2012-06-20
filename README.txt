Create a config file called icl.cfg in ~/.icinga/ or /etc/icinga/ containing 
your Icinga-web API url and and API-key which is allowed to access it.


Usage: icl [options]

Options:
  -h, --help            show this help message and exit
  -s HOSTNAME[,HOSTNAME], --system=HOSTNAME[,HOSTNAME], --host=HOSTNAME[,HOSTNAME]
                        Selects the host with this name
  -f HOSTGROUPNAME[,HOSTGROUPNAME], --function=HOSTGROUPNAME[,HOSTGROUPNAME], --hostgroup=HOSTGROUPNAME[,HOSTGROUPNAME]
                        Selects all hosts in the hostgroup with this name
  --service=[<service name>/host]
                        Specifies the service to which an action should be
                        performed. When not specified, all services will be
                        selected
  -a <action>, --action=<action>
                        Action to be performed on specified service/host:
                        - status (default):                Show status info
                        - check:                           Perform a check
                        - alerts-off (off):                Turn alerts off
                        - alerts-on (on):                  Turn alerts on
                        - checks-off:                      Turn checks off
                        - checks-on:                       Turn checks on
                        - acknowledge (ack):               Acknowledge problem
                        - remove-acknowledgement (remove-ack): Remove an ack
  --force               Force the check of the specified service/host
                        (Note: this will also force a check of passive checks!
  --openproblems        Shows you all open problems
  --allproblems         Shows you all problems
  -l LOGLEVEL, --loglevel=LOGLEVEL
                        loglevel for the script, defaults to INFO
  --silence             Globally turns off notifications on all instances
  --noise               Globally turns on notifications on all instances