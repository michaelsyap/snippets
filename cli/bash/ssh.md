# SSH

## SSH Tunnelling
ssh -L local_mysql_port_pointing_to_remote_sql_port:local_ip_address_of_mysql_inside_remote:mysql_remote_port -p 5069  root@remoete_server_ip_address



## Connecting to MYSQL to SSH tunneled MYSQL server
mysql -h --host=127.0.0.1 --port=local_mysql_port_pointing_to_remote_sql_port -u root -p
mysql -h remote_ip_address --port=local_mysql_port_pointing_to_remote_sql_port -u root -p