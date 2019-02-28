# Mariadb Role

This ansible role will:
<ul>
  <li>Install MariaDB packages from the official MariaDB repositories</li>
  <li>Set database root password for the hosts: <strong>localhost</strong>, <strong>127.0.0.1</strong>, <strong>::1</strong></li>
  <li>Remove anonymous users</li>
  <li>Remove test database</li>
  <li>Modify configuration file <strong>server.cnf</strong> to listen on all interfaces <strong>0.0.0.0</strong>
  </ul>

# Requirements
No specific requirements

# Role Variables

<u>
  <li><strong>mariadb_root_password</strong>: The MariaDB root password, change it with your own password.</li>
  <li><strong>mariadb_version</strong>:The version of MariaDB to be installed.</li>
  <li><strong>mariadb_packages</strong>: Install the required packages; MariaDB-server, MySQL-python</li>
</u>

# Test


$ ansible-playbook -i inventory.ini test-mariadb.yml
