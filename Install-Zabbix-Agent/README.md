# Ansible-Role-ZabbixAgent

# Requirements

To be able to add, remove, update the hosts on the zabbix server you need to install <strong>zabbix-api</strong> package, use the following command to install it locally:
</br>
$ pip install zabbix-api

# Role Variables

<ul>
  <li><strong>zabbix_version</strong>: Version of Zabbix Agent</strong></li>
  <li><strong>zabbix_server_ip</strong>: Zabbix server IP or the Zabbix proxy IP </li>
  <li><strong>zabbix_active_server_ip</strong>: Active zabbix server IP</li>
    </ul>
 </br>
 
 <h3>Zabbix API Variables</h3>
 <ul>
  <li><strong>zabbix_url</strong>: Zabbix API Frontend URL</li>
  <li><strong>zabbix_api_user</strong>: Zabbix API User
  <li><strong>zabbix_api_pass</strong>: Zabbix API Password</li>
  <li><strong>zabbix_agent_hostname</strong>: Zabbix Agent Hostname Node</li>
  <li><strong>zabbix_host_groups</strong>: Zabbix host groups to be inserted into</li>
  <li><strong>zabbix_link_templates</strong>: Zabbix Templates to be associated </li>
  <li><strong>zabbix_create_host</strong>: can be present or absent variable to add/update a node or remove an existant node</li> 
  </ul>
    
# Test
$ ansible-playbook -i inventory.ini test-zabbix-agent.yml
