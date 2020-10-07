# zabbix-ossec-hids-server-template
Created and tested on zabbix 5 on FreeBSD.
# Installation procedure:
1. Include ossec.conf in zabbix agent configuration on OSSEC-HIDS server;
2. Configure sudoers to allow zabbix account to run list_agents and agent_control (see ossec.conf);
3. Import zabbix_ossec-hids_server_template.xml on zabbix server and link it to OSSEC-HIDS server host.
# Template functionality:
Items:
 - Number of connected OSSEC-HIDS agents
 - Number of disconnected OSSEC-HIDS agents
 - Total number of OSSEC agents
Autodiscovery:
 - automatic discovery of configured OSSEC-HIDS agents
 - automated trigger creation (for OSSEC agents 'Disconnected' state)
# Usage on *BSD and non-BSD UNIX-like systems
ON BSD systems should work without modifications.
On non-BSD it might be required to change path to binaries in ossec.conf.
