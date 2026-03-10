# Monitoring Architecture

This project implements a centralized monitoring setup using Zabbix.

## Components

Zabbix Server
- Installed on Ubuntu virtual machine
- Responsible for collecting and storing monitoring data

Monitored Hosts
- Windows Host 1 with Zabbix Agent
- Windows Host 2 with Zabbix Agent

## Monitoring Flow

1. Zabbix agents run on monitored machines.
2. Agents collect system metrics such as CPU, memory, disk usage and uptime.
3. These metrics are sent to the Zabbix server.
4. The Zabbix server stores the data in its database.
5. The data is visualized through the Zabbix web dashboard.

## Communication

Agents communicate with the Zabbix server using the default Zabbix ports.

Agent port: 10050  
Server port: 10051
